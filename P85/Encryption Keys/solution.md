## CPP

### SOLUTION

int countCoprimeSubsequences(int n, vector<int>& a) {
    const int MOD = 1000000007;
    const int MAX_VAL = 100000;
    
    vector<int> cnt(MAX_VAL + 1, 0);
    for (int x : a) {
        if (x <= MAX_VAL) {
            cnt[x]++;
        }
    }

    vector<int> multiples_count(MAX_VAL + 1, 0);
    for (int i = 1; i <= MAX_VAL; ++i) {
        for (int j = i; j <= MAX_VAL; j += i) {
            multiples_count[i] += cnt[j];
        }
    }

    vector<long long> pow2(n + 1);
    pow2[0] = 1;
    for (int i = 1; i <= n; ++i) {
        pow2[i] = (pow2[i - 1] * 2) % MOD;
    }

    vector<long long> dp(MAX_VAL + 1);
    for (int i = MAX_VAL; i >= 1; --i) {
        int count = multiples_count[i];
        if (count == 0) {
            dp[i] = 0;
            continue;
        }
        long long total = (pow2[count] - 1 + MOD) % MOD;
        for (int j = 2 * i; j <= MAX_VAL; j += i) {
            total = (total - dp[j] + MOD) % MOD;
        }
        
        dp[i] = total;
    }

    return dp[1];
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION


public static int countCoprimeSubsequences(int n, int[] a) {
    int MOD = 1000000007;
    int MAX_VAL = 100000;
    
    int[] cnt = new int[MAX_VAL + 1];
    for (int x : a) {
        if (x <= MAX_VAL) {
            cnt[x]++;
        }
    }
    
    int[] multiplesCount = new int[MAX_VAL + 1];
    for (int i = 1; i <= MAX_VAL; i++) {
        for (int j = i; j <= MAX_VAL; j += i) {
            multiplesCount[i] += cnt[j];
        }
    }
    
    long[] pow2 = new long[n + 1];
    pow2[0] = 1;
    for (int i = 1; i <= n; i++) {
        pow2[i] = (pow2[i - 1] * 2) % MOD;
    }
    
    long[] dp = new long[MAX_VAL + 1];
    for (int i = MAX_VAL; i >= 1; i--) {
        int count = multiplesCount[i];
        if (count == 0) {
            dp[i] = 0;
            continue;
        }
        
        long total = (pow2[count] - 1 + MOD) % MOD;
        
        for (int j = 2 * i; j <= MAX_VAL; j += i) {
            total = (total - dp[j] + MOD) % MOD;
        }
        dp[i] = total;
    }
    
    return (int) dp[1];
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


