## CPP

### SOLUTION

long long dp[10005][100][2];
long long MOD = 1000000007;

long long digit_dp(std::string &s, int idx, int sum_mod, int d, bool tight) {
    if (idx == s.size()) {
        return (sum_mod % d == 0);
    }
    if (dp[idx][sum_mod][tight] != -1) {
        return dp[idx][sum_mod][tight];
    }

    long long res = 0;
    int limit = (tight ? s[idx] - '0' : 9);

    for (int i = 0; i <= limit; ++i) {
        res += digit_dp(s, idx + 1, (sum_mod + i) % d, d, (tight && (s[idx] - '0' == i)));
        res %= MOD;
    }

    return dp[idx][sum_mod][tight] = res;
}

long long countAccessCodes(string K, int D) {
    
    int n = K.size();
    memset(dp, -1, sizeof(dp));
    
    long long res = digit_dp(K, 0, 0, D, true);

    return (res - 1 + MOD) % MOD;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

long[][][] dp;
long MOD = 1000000007;
int D_val;
String K_str;

long digit_dp(int idx, int sum_mod, int tight) {
    if (idx == K_str.length()) {
        return (sum_mod % D_val == 0) ? 1 : 0;
    }
    if (dp[idx][sum_mod][tight] != -1) {
        return dp[idx][sum_mod][tight];
    }

    long res = 0;
    int limit = (tight == 1 ? K_str.charAt(idx) - '0' : 9);

    for (int i = 0; i <= limit; ++i) {
        int next_tight = (tight == 1 && (K_str.charAt(idx) - '0' == i)) ? 1 : 0;
        res += digit_dp(idx + 1, (sum_mod + i) % D_val, next_tight);
        res %= MOD;
    }

    return dp[idx][sum_mod][tight] = res;
}

public long countAccessCodes(String K, int D) {
    this.K_str = K;
    this.D_val = D;
    int n = K.length();
    dp = new long[n + 1][D][2];
    
    for (int i = 0; i <= n; i++) {
        for (int j = 0; j < D; j++) {
            dp[i][j][0] = -1;
            dp[i][j][1] = -1;
        }
    }

    long res = digit_dp(0, 0, 1);
    return (res - 1 + MOD) % MOD;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


