## CPP

### SOLUTION

long long solve(string s) {
    int n = s.length();
    long long MOD = 1e9 + 7;
    vector<long long> dp(n + 1, 0);
    dp[0] = 1;
    vector<int> last_occurrence(256, -1);

    for (int i = 1; i <= n; ++i) {
        char currentChar = s[i - 1];
        dp[i] = (2 * dp[i - 1]) % MOD;

        if (last_occurrence[currentChar] != -1) {
            int prevIdx = last_occurrence[currentChar];
            dp[i] = (dp[i] - dp[prevIdx - 1] + MOD) % MOD;
        }
        last_occurrence[currentChar] = i;
    }
    return (dp[n] - 1 + MOD) % MOD;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static long solve(String s) {
    int n = s.length();
    long MOD = 1_000_000_007L;
    long[] dp = new long[n + 1];
    dp[0] = 1;
    int[] lastOccurrence = new int[256];
    java.util.Arrays.fill(lastOccurrence, -1);

    for (int i = 1; i <= n; ++i) {
        char currentChar = s.charAt(i - 1);
        dp[i] = (2 * dp[i - 1]) % MOD;

        if (lastOccurrence[currentChar] != -1) {
            int prevIdx = lastOccurrence[currentChar];
            dp[i] = (dp[i] - dp[prevIdx - 1] + MOD) % MOD;
        }
        lastOccurrence[currentChar] = i;
    }
    return (dp[n] - 1 + MOD) % MOD;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  

