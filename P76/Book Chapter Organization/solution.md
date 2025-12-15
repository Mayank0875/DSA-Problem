## CPP

### SOLUTION

long long minTotalStress(int n, int k, const vector<int>& pulses) {
    typedef long long ll;
    const ll INF = (ll)1e18;

    vector<ll> x(n + 1, 0);
    vector<ll> prefix_sum(n + 1, 0);
    vector<ll> dp_prev(n + 1, INF);
    vector<ll> dp_curr(n + 1, INF);

    auto cost = [&](int l, int r) -> ll {
        ll s = prefix_sum[r] - prefix_sum[l - 1];
        return s * s;
    };

    for (int i = 0; i < n; i++) {
        x[i + 1] = pulses[i];
        prefix_sum[i + 1] = prefix_sum[i] + x[i + 1];
    }
    dp_prev[0] = 0;
    for (int i = 1; i <= n; i++) {
        dp_prev[i] = cost(1, i);
    }

    function<void(int,int,int,int)> compute =
    [&](int l, int r, int optl, int optr) {
        if (l > r) return;

        int mid = (l + r) / 2;
        pair<ll, int> best = {INF, -1};

        int end_search = min(mid - 1, optr);
        for (int i = optl; i <= end_search; i++) {
            ll val = dp_prev[i] + cost(i + 1, mid);
            if (val < best.first) {
                best = {val, i};
            }
        }

        dp_curr[mid] = best.first;
        int opt = best.second;

        compute(l, mid - 1, optl, opt);
        compute(mid + 1, r, opt, optr);
    };

    for (int grp = 2; grp <= k; grp++) {
        compute(1, n, 0, n - 1);
        dp_prev = dp_curr;
    }

    return dp_prev[n];
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static long minTotalStress(int n, int k, int[] pulses) {
    final long INF = 1_000_000_000_000_000_000L;

    long[] prefixSum = new long[n + 1];
    long[] dpPrev = new long[n + 1];
    long[] dpCurr = new long[n + 1];

    // prefix sum
    for (int i = 0; i < n; i++) {
        prefixSum[i + 1] = prefixSum[i] + pulses[i];
    }

    // cost function
    java.util.function.BiFunction<Integer, Integer, Long> cost =
        (l, r) -> {
            long s = prefixSum[r] - prefixSum[l - 1];
            return s * s;
        };

    // base case k = 1
    for (int i = 1; i <= n; i++) {
        dpPrev[i] = cost.apply(1, i);
    }

    // divide & conquer compute
    class DnC {
        void compute(int l, int r, int optl, int optr) {
            if (l > r) return;

            int mid = (l + r) / 2;
            long bestVal = INF;
            int bestK = -1;

            int endSearch = Math.min(mid - 1, optr);
            for (int i = optl; i <= endSearch; i++) {
                long val = dpPrev[i] + cost.apply(i + 1, mid);
                if (val < bestVal) {
                    bestVal = val;
                    bestK = i;
                }
            }

            dpCurr[mid] = bestVal;
            int opt = bestK;

            compute(l, mid - 1, optl, opt);
            compute(mid + 1, r, opt, optr);
        }
    }

    DnC solver = new DnC();

    // DP layers
    for (int grp = 2; grp <= k; grp++) {
        solver.compute(1, n, 0, n - 1);
        System.arraycopy(dpCurr, 0, dpPrev, 0, n + 1);
    }

    return dpPrev[n];
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  
