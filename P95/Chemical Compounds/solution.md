## CPP

### SOLUTION

int countDistinctMultisets(int n, const std::vector<int>& a) {
    map<int, int> counts;
    int max_cnt = 0;
    for (int x : a) {
        counts[x]++;
        if (counts[x] > max_cnt) {
            max_cnt = counts[x];
        }
    }

    vector<long long> dp(n + 1, 0);
    dp[0] = 1;
    long long P = 998244353;

    for (auto const& [val, count] : counts) {
        for (int j = n; j >= count; --j) {
            dp[j] = (dp[j] + (long long)count * dp[j - count]) % P;
        }
    }

    long long ans = 0;
    for (int i = max_cnt; i <= n; ++i) {
        ans = (ans + dp[i]) % P;
    }
    return (int)ans;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static int countDistinctMultisets(int n, int[] a) {
    java.util.Map<Integer, Integer> counts = new java.util.HashMap<>();
    int max_cnt = 0;
    for (int x : a) {
        int c = counts.getOrDefault(x, 0) + 1;
        counts.put(x, c);
        if (c > max_cnt) {
            max_cnt = c;
        }
    }

    long[] dp = new long[n + 1];
    dp[0] = 1;
    long P = 998244353L;

    for (int count : counts.values()) {
        for (int j = n; j >= count; --j) {
            dp[j] = (dp[j] + count * dp[j - count]) % P;
        }
    }

    long ans = 0;
    for (int i = max_cnt; i <= n; ++i) {
        ans = (ans + dp[i]) % P;
    }
    return (int)ans;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  

