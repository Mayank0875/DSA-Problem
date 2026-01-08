## CPP

### SOLUTION

const int MOD = 1e9 + 7;

int countWays(int n) {
    if (n == 1) return 1;
    if (n == 2) return 2; // 1+1, 2

    vector<vector<long long>> dp(n + 1, vector<long long>(2));

    dp[1][0] = 1; 
    dp[1][1] = 0;

    dp[2][0] = 1; 
    dp[2][1] = 1;

    for (int i = 3; i <= n; i++) {
        dp[i][0] = (dp[i - 1][0] + dp[i - 1][1]) % MOD;
        dp[i][1] = dp[i - 2][0];
    }

    return (dp[n][0] + dp[n][1]) % MOD;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

static final int MOD = 1000000007;

public static int countWays(int n) {
    if (n == 1) return 1;
    if (n == 2) return 2;

    long[][] dp = new long[n + 1][2];

    // dp[i][0] -> last jump was +1
    // dp[i][1] -> last jump was +2

    dp[1][0] = 1;
    dp[1][1] = 0;

    dp[2][0] = 1;
    dp[2][1] = 1;

    for (int i = 3; i <= n; i++) {
        dp[i][0] = (dp[i - 1][0] + dp[i - 1][1]) % MOD;
        dp[i][1] = dp[i - 2][0];
    }

    return (int)((dp[n][0] + dp[n][1]) % MOD);
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

#define MOD 1000000007

int countWays(int n) {
    if (n == 1) return 1;
    if (n == 2) return 2;

    long long dp[n + 1][2];

    for (int i = 0; i <= n; i++) {
        dp[i][0] = dp[i][1] = 0;
    }

    dp[1][0] = 1;
    dp[1][1] = 0;

    dp[2][0] = 1;
    dp[2][1] = 1;

    for (int i = 3; i <= n; i++) {
        dp[i][0] = (dp[i - 1][0] + dp[i - 1][1]) % MOD;
        dp[i][1] = dp[i - 2][0];
    }

    return (dp[n][0] + dp[n][1]) % MOD;
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

const MOD = 1000000007;

function countWays(n) {
    if (n === 1) return 1;
    if (n === 2) return 2;

    let dp = Array.from({ length: n + 1 }, () => [0, 0]);

    // dp[i][0] -> last jump was +1
    // dp[i][1] -> last jump was +2

    dp[1][0] = 1;
    dp[1][1] = 0;

    dp[2][0] = 1;
    dp[2][1] = 1;

    for (let i = 3; i <= n; i++) {
        dp[i][0] = (dp[i - 1][0] + dp[i - 1][1]) % MOD;
        dp[i][1] = dp[i - 2][0];
    }

    return (dp[n][0] + dp[n][1]) % MOD;
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def countWays(n: int) -> int:
    MOD = 10**9 + 7

    if n == 1:
        return 1
    if n == 2:
        return 2

    dp = [[0, 0] for _ in range(n + 1)]

    # dp[i][0] -> last jump was +1
    # dp[i][1] -> last jump was +2

    dp[1][0] = 1
    dp[1][1] = 0

    dp[2][0] = 1
    dp[2][1] = 1

    for i in range(3, n + 1):
        dp[i][0] = (dp[i - 1][0] + dp[i - 1][1]) % MOD
        dp[i][1] = dp[i - 2][0]

    return (dp[n][0] + dp[n][1]) % MOD


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  