## CPP

### SOLUTION

string solvePartition(string s) {
    int n = s.length();
    if (n < 3) return "No";

    vector<vector<bool>> isPal(n, vector<bool>(n, false));
    for (int len = 1; len <= n; ++len) {
        for (int i = 0; i <= n - len; ++i) {
            int j = i + len - 1;
            if (len == 1) {
                isPal[i][j] = true;
            } else if (len == 2) {
                isPal[i][j] = (s[i] == s[j]);
            } else {
                isPal[i][j] = (s[i] == s[j]) && isPal[i + 1][j - 1];
            }
        }
    }

    for (int i = 0; i < n - 2; ++i) {
        if (isPal[0][i]) {
            for (int j = i + 1; j < n - 1; ++j) {
                if (isPal[i + 1][j] && isPal[j + 1][n - 1]) {
                    return "Yes";
                }
            }
        }
    }

    return "No";
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static String solvePartition(String s) {
    int n = s.length();
    if (n < 3) return "No";

    boolean[][] isPal = new boolean[n][n];
    for (int len = 1; len <= n; ++len) {
        for (int i = 0; i <= n - len; ++i) {
            int j = i + len - 1;
            if (len == 1) {
                isPal[i][j] = true;
            } else if (len == 2) {
                isPal[i][j] = (s.charAt(i) == s.charAt(j));
            } else {
                isPal[i][j] = (s.charAt(i) == s.charAt(j)) && isPal[i + 1][j - 1];
            }
        }
    }

    for (int i = 0; i < n - 2; ++i) {
        if (isPal[0][i]) {
            for (int j = i + 1; j < n - 1; ++j) {
                if (isPal[i + 1][j] && isPal[j + 1][n - 1]) {
                    return "Yes";
                }
            }
        }
    }

    return "No";
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

bool isPalindrome(char* s, int i, int j) {
    while (i < j) {
        if (s[i] != s[j]) {
            return false;
        }
        i++;
        j--;
    }
    return true;
}

char* solvePartition(char* s) {
    int n = strlen(s);
    if (n < 3) return "No";

    bool isPal[n][n];
    memset(isPal, 0, sizeof(isPal));
    for (int len = 1; len <= n; ++len) {
        for (int i = 0; i <= n - len; ++i) {
            int j = i + len - 1;
            if (len == 1) {
                isPal[i][j] = true;
            } else if (len == 2) {
                isPal[i][j] = (s[i] == s[j]);
            } else {
                isPal[i][j] = (s[i] == s[j]) && isPal[i + 1][j - 1];
            }
        }
    }

    for (int i = 0; i < n - 2; ++i) {
        if (isPal[0][i]) {
            for (int j = i + 1; j < n - 1; ++j) {
                if (isPal[i + 1][j] && isPal[j + 1][n - 1]) {
                    return "Yes";
                }
            }
        }
    }

    return "No";
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function solvePartition(s) {
    const n = s.length;
    if (n < 3) return "No";

    const isPal = Array.from({ length: n }, () => Array(n).fill(false));
    for (let len = 1; len <= n; ++len) {
        for (let i = 0; i <= n - len; ++i) {
            const j = i + len - 1;
            if (len === 1) {
                isPal[i][j] = true;
            } else if (len === 2) {
                isPal[i][j] = (s[i] === s[j]);
            } else {
                isPal[i][j] = (s[i] === s[j]) && isPal[i + 1][j - 1];
            }
        }
    }

    for (let i = 0; i < n - 2; ++i) {
        if (isPal[0][i]) {
            for (let j = i + 1; j < n - 1; ++j) {
                if (isPal[i + 1][j] && isPal[j + 1][n - 1]) {
                    return "Yes";
                }
            }
        }
    }

    return "No";
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def solvePartition(s):
    n = len(s)
    if n < 3:
        return "No"

    is_pal = [[False] * n for _ in range(n)]
    for length in range(1, n + 1):
        for i in range(n - length + 1):
            j = i + length - 1
            if length == 1:
                is_pal[i][j] = True
            elif length == 2:
                is_pal[i][j] = (s[i] == s[j])
            else:
                is_pal[i][j] = (s[i] == s[j]) and is_pal[i + 1][j - 1]

    for i in range(n - 2):
        if is_pal[0][i]:
            for j in range(i + 1, n - 1):
                if is_pal[i + 1][j] and is_pal[j + 1][n - 1]:
                    return "Yes"

    return "No"

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  