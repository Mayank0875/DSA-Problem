## CPP

### SOLUTION

long long dp[20][11][2][2];

long long digit_dp(std::string &s, int idx, int prev, bool tight, bool zero) {
    if (idx == s.size()) {
        return 1;
    }
    if (dp[idx][prev][tight][zero] != -1) {
        return dp[idx][prev][tight][zero];
    }
    long long res = 0;
    int limit = (tight ? s[idx] - '0' : 9);
    for (int i = 0; i <= limit; ++i) {
        if (i == prev && !zero) continue;
        
        bool next_tight = tight && (i == limit);
        bool next_zero = zero && (i == 0);
        
        int next_prev = next_zero ? 10 : i;

        res += digit_dp(s, idx + 1, next_prev, next_tight, next_zero);
    }
    return dp[idx][prev][tight][zero] = res;
}

long long count(long long n) {
    if (n < 0) return 0;
    if (n == 0) return 1; 
    std::string s = std::to_string(n);
    memset(dp, -1, sizeof(dp));
    return digit_dp(s, 0, 10, true, true);
}

long long countValidIntegers(long long a, long long b) {
    return count(b) - count(a - 1);
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

long[][][][] dp;

long digit_dp(String s, int idx, int prev, int tight, int zero) {
    if (idx == s.length()) {
        return 1;
    }
    if (dp[idx][prev][tight][zero] != -1) {
        return dp[idx][prev][tight][zero];
    }

    long res = 0;
    int limit = (tight == 1 ? s.charAt(idx) - '0' : 9);

    for (int i = 0; i <= limit; ++i) {
        if (i == prev && zero == 0) continue;

        int next_tight = (tight == 1 && i == limit) ? 1 : 0;
        int next_zero = (zero == 1 && i == 0) ? 1 : 0;
        int next_prev = (next_zero == 1) ? 10 : i;

        res += digit_dp(s, idx + 1, next_prev, next_tight, next_zero);
    }

    return dp[idx][prev][tight][zero] = res;
}

long count(long n) {
    if (n < 0) return 0;
    if (n == 0) return 1;
    String s = String.valueOf(n);
    
    dp = new long[20][11][2][2];
    for(int i=0; i<20; i++) {
        for(int j=0; j<11; j++) {
            for(int k=0; k<2; k++) {
                for(int l=0; l<2; l++) {
                    dp[i][j][k][l] = -1;
                }
            }
        }
    }
    
    return digit_dp(s, 0, 10, 1, 1);
}

public long countValidIntegers(long a, long b) {
    return count(b) - count(a - 1);
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  
