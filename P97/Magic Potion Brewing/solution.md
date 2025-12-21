## CPP

### SOLUTION

long long countBalancedSubarrays(int n, std::vector<int> a) {
    std::vector<int> a1(n, 0), a2(n, 0);
    for (int i = 0; i < n; i++) {
        if (a[i] == 1) a1[i] = 1;
        if (a[i] == 2) a2[i] = 1;
    }

    std::vector<long long> pref(n + 1, 0);
    std::vector<int> pref1(n + 1, 0), pref2(n + 1, 0);

    for (int i = 0; i < n; i++) {
        pref[i + 1] = pref[i] + a[i];
        pref1[i + 1] = pref1[i] + a1[i];
        pref2[i + 1] = pref2[i] + a2[i];
    }

    long long ans = 0;

    for (int i = 0; i < n; i++) {
        int l = i - 1, r = n + 1;
        while (r - l > 1) {
            int mid = (r + l) / 2;
            if (pref[mid] - pref[i] >= 3) r = mid;
            else l = mid;
        }

        if (r <= n && pref[r] - pref[i] == 3 && 
            pref1[r] - pref1[i] == 1 && pref2[r] - pref2[i] == 1) {
            
            int x = r;
            l = r; 
            r = n + 1;
            while (r - l > 1) {
                int mid = (r + l) / 2;
                if (pref[mid] - pref[i] > 3) r = mid;
                else l = mid;
            }
            
            if (x - i == 2) {
                ans += (r - x - 1);
            } else {
                ans += (r - x);
            }
        }
    }

    for (int i = 0; i < n; i++) {
        int l = i - 1, r = n + 1;
        while (r - l > 1) {
            int mid = (r + l) / 2;
            if (pref[mid] - pref[i] >= 2) r = mid;
            else l = mid;
        }

        if (r <= n && pref[r] - pref[i] == 2 && pref1[r] - pref1[i] == 2) {
            int x = r;
            l = r; 
            r = n + 1;
            while (r - l > 1) {
                int mid = (r + l) / 2;
                if (pref[mid] - pref[i] > 2) r = mid;
                else l = mid;
            }
            
            if (x - i == 2) {
                ans += (r - x - 1);
            } else {
                ans += (r - x);
            }
        }
    }

    return ans;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static long countBalancedSubarrays(int n, int[] a) {
    int[] a1 = new int[n];
    int[] a2 = new int[n];
    for (int i = 0; i < n; i++) {
        if (a[i] == 1) a1[i] = 1;
        if (a[i] == 2) a2[i] = 1;
    }

    long[] pref = new long[n + 1];
    int[] pref1 = new int[n + 1];
    int[] pref2 = new int[n + 1];

    for (int i = 0; i < n; i++) {
        pref[i + 1] = pref[i] + a[i];
        pref1[i + 1] = pref1[i] + a1[i];
        pref2[i + 1] = pref2[i] + a2[i];
    }

    long ans = 0;

    for (int i = 0; i < n; i++) {
        int l = i - 1, r = n + 1;
        while (r - l > 1) {
            int mid = (r + l) / 2;
            if (pref[mid] - pref[i] >= 3) r = mid;
            else l = mid;
        }

        if (r <= n && pref[r] - pref[i] == 3 && 
            pref1[r] - pref1[i] == 1 && pref2[r] - pref2[i] == 1) {
            
            int x = r;
            l = r; r = n + 1;
            while (r - l > 1) {
                int mid = (r + l) / 2;
                if (pref[mid] - pref[i] > 3) r = mid;
                else l = mid;
            }
            
            if (x - i == 2) ans += (r - x - 1);
            else ans += (r - x);
        }
    }
    for (int i = 0; i < n; i++) {
        int l = i - 1, r = n + 1;
        while (r - l > 1) {
            int mid = (r + l) / 2;
            if (pref[mid] - pref[i] >= 2) r = mid;
            else l = mid;
        }

        if (r <= n && pref[r] - pref[i] == 2 && pref1[r] - pref1[i] == 2) {
            int x = r;
            l = r; r = n + 1;
            while (r - l > 1) {
                int mid = (r + l) / 2;
                if (pref[mid] - pref[i] > 2) r = mid;
                else l = mid;
            }
            
            if (x - i == 2) ans += (r - x - 1);
            else ans += (r - x);
        }
    }

    return ans;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  

