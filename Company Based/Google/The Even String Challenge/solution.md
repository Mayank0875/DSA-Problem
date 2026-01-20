## CPP

### SOLUTION

int solve(const string& s, int idx, int pre, vector<vector<int>>& dp) {
    if (idx == s.size()) {
        return (pre != 26) ? 1 : 0;
    }
    if (dp[idx][pre] != -1) return dp[idx][pre];

    int res;
    if (pre == 26) {
        int deleteChar = 1 + solve(s, idx + 1, 26, dp);
        int keepChar = solve(s, idx + 1, s[idx] - 'a', dp);
        res = min(deleteChar, keepChar);
    } else {
        if ((s[idx] - 'a') == pre) {
            res = solve(s, idx + 1, 26, dp);
        } else {
            res = 1 + solve(s, idx + 1, pre, dp);
        }
    }
    return dp[idx][pre] = res;
}

int minRemovals(string s) {
    int n = s.size();
    vector<vector<int>> dp(n, vector<int>(27, -1));
    return solve(s, 0, 26, dp);
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static int solve(String s, int idx, int pre, Integer[][] dp) {
    if (idx == s.length()) {
        return (pre != 26) ? 1 : 0;
    }
    if (dp[idx][pre] != null) return dp[idx][pre];

    int res;
    if (pre == 26) {
        int deleteChar = 1 + solve(s, idx + 1, 26, dp);
        int keepChar = solve(s, idx + 1, s.charAt(idx) - 'a', dp);
        res = Math.min(deleteChar, keepChar);
    } else {
        if ((s.charAt(idx) - 'a') == pre) {
            res = solve(s, idx + 1, 26, dp);
        } else {
            res = 1 + solve(s, idx + 1, pre, dp);
        }
    }
    return dp[idx][pre] = res;
}

public static int minRemovals(String s) {
    int n = s.length();
    Integer[][] dp = new Integer[n][27];
    return solve(s, 0, 26, dp);
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

#define MIN(a,b) (((a)<(b))?(a):(b))

int memo[200005][27];
char* strPtr;
int len;

int solve(int idx, int pre) {
    if (idx == len) {
        return (pre != 26) ? 1 : 0;
    }
    if (memo[idx][pre] != -1) return memo[idx][pre];

    int res;
    if (pre == 26) {
        // Delete current
        int res1 = 1 + solve(idx + 1, 26);
        // Keep current
        int res2 = solve(idx + 1, strPtr[idx] - 'a');
        res = MIN(res1, res2);
    } else {
        if ((strPtr[idx] - 'a') == pre) {
            // Match found
            res = solve(idx + 1, 26);
        } else {
            // Must delete
            res = 1 + solve(idx + 1, pre);
        }
    }
    return memo[idx][pre] = res;
}

int minRemovals(char* s) {
    strPtr = s;
    len = strlen(s);
    // Initialize memo table for this test case
    for(int i = 0; i < len; i++) {
        for(int j = 0; j < 27; j++) {
            memo[i][j] = -1;
        }
    }
    return solve(0, 26);
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function minRemovals(s) {
    const n = s.length;
    const dp = Array.from({ length: n }, () => Array(27).fill(-1));

    function solve(idx, pre) {
        if (idx === n) {
            return (pre !== 26) ? 1 : 0;
        }
        if (dp[idx][pre] !== -1) return dp[idx][pre];

        let res;
        if (pre === 26) {
            const deleteChar = 1 + solve(idx + 1, 26);
            const keepChar = solve(idx + 1, s.charCodeAt(idx) - 97);
            res = Math.min(deleteChar, keepChar);
        } else {
            if ((s.charCodeAt(idx) - 97) === pre) {
                res = solve(idx + 1, 26);
            } else {
                res = 1 + solve(idx + 1, pre);
            }
        }
        return dp[idx][pre] = res;
    }

    return solve(0, 26);
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def minRemovals(s: str) -> int:
    n = len(s)
    dp = [[-1] * 27 for _ in range(n)]

    def solve(idx, pre):
        if idx == n:
            return 1 if pre != 26 else 0
        
        if dp[idx][pre] != -1:
            return dp[idx][pre]
        
        res = 0
        if pre == 26:
            res1 = 1 + solve(idx + 1, 26)
            res2 = solve(idx + 1, ord(s[idx]) - ord('a'))
            res = min(res1, res2)
        else:
            if (ord(s[idx]) - ord('a')) == pre:
                res = solve(idx + 1, 26)
            else:
                res = 1 + solve(idx + 1, pre)
        
        dp[idx][pre] = res
        return res

    return solve(0, 26)

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  