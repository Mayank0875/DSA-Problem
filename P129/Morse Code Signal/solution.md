## CPP

### SOLUTION

int countSubsequences(string s, string t) {
    int m = s.length();
    int n = t.length();
    int MOD = 1e9 + 7;
    
    // dp[i][j] stores the number of ways to form s[0...i-1] from t[0...j-1]
    vector<vector<int>> dp(m + 1, vector<int>(n + 1));
    
    // An empty s is a subsequence of any prefix of t exactly once
    for (int j = 0; j <= n; j++) {
        dp[0][j] = 1;
    }
    
    for (int i = 1; i <= m; i++) {
        for (int j = 1; j <= n; j++) {
            if (s[i - 1] == t[j - 1]) {
                // If characters match, we can either use this character or ignore it
                dp[i][j] = (dp[i][j - 1] + dp[i - 1][j - 1]) % MOD;
            } else {
                // If characters don't match, we must ignore the current character of t
                dp[i][j] = dp[i][j - 1];
            }
        }
    }
    
    return dp[m][n];
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static int countSubsequences(String s, String t) {
    int m = s.length();
    int n = t.length();
    int MOD = 1000000007;
    
    int[][] dp = new int[m + 1][n + 1];
    
    for (int j = 0; j <= n; j++) {
        dp[0][j] = 1;
    }
    
    for (int i = 1; i <= m; i++) {
        for (int j = 1; j <= n; j++) {
            if (s.charAt(i - 1) == t.charAt(j - 1)) {
                dp[i][j] = (dp[i][j - 1] + dp[i - 1][j - 1]) % MOD;
            } else {
                dp[i][j] = dp[i][j - 1];
            }
        }
    }
    
    return dp[m][n];
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

int countSubsequences(char* s, char* t) {
    int m = strlen(s);
    int n = strlen(t);
    int MOD = 1000000007;
    
    // Using simple 2D array allocation
    int** dp = (int**)malloc((m + 1) * sizeof(int*));
    for (int i = 0; i <= m; i++) {
        dp[i] = (int*)malloc((n + 1) * sizeof(int));
    }
    
    for (int j = 0; j <= n; j++) dp[0][j] = 1;
    for (int i = 1; i <= m; i++) dp[i][0] = 0;
    
    for (int i = 1; i <= m; i++) {
        for (int j = 1; j <= n; j++) {
            if (s[i - 1] == t[j - 1]) {
                dp[i][j] = (dp[i][j - 1] + dp[i - 1][j - 1]) % MOD;
            } else {
                dp[i][j] = dp[i][j - 1];
            }
        }
    }
    
    int result = dp[m][n];
    
    for (int i = 0; i <= m; i++) free(dp[i]);
    free(dp);
    
    return result;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function countSubsequences(s, t) {
    const m = s.length;
    const n = t.length;
    const MOD = 1000000007;
    
    // Create (m+1) x (n+1) grid initialized to 0
    let dp = Array(m + 1).fill().map(() => Array(n + 1).fill(0));
    
    for (let j = 0; j <= n; j++) {
        dp[0][j] = 1;
    }
    
    for (let i = 1; i <= m; i++) {
        for (let j = 1; j <= n; j++) {
            if (s[i - 1] === t[j - 1]) {
                dp[i][j] = (dp[i][j - 1] + dp[i - 1][j - 1]) % MOD;
            } else {
                dp[i][j] = dp[i][j - 1];
            }
        }
    }
    
    return dp[m][n];
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def countSubsequences(s: str, t: str) -> int:
    m, n = len(s), len(t)
    MOD = 10**9 + 7
    
    dp = [[0] * (n + 1) for _ in range(m + 1)]
    
    for j in range(n + 1):
        dp[0][j] = 1
        
    for i in range(1, m + 1):
        for j in range(1, n + 1):
            if s[i - 1] == t[j - 1]:
                dp[i][j] = (dp[i][j - 1] + dp[i - 1][j - 1]) % MOD
            else:
                dp[i][j] = dp[i][j - 1]
                
    return dp[m][n]
    
### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  