## CPP

### SOLUTION

int killDemodogs(int n) {
    long long N = n;
    long long MOD = 1e9 + 7;
    
    long long term1 = (N * (N + 1)) % MOD;
    long long term2 = (4 * N - 1) % MOD;
    
    long long ans = (term1 * term2) % MOD;
    ans = (ans * 337) % MOD;
    
    return (int)ans;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static int killDemodogs(int n) {
    long N = n;
    long MOD = 1000000007L;
    
    // Formula derived: n * (n+1) * (4n-1) * 337 % MOD
    long term1 = (N * (N + 1)) % MOD;
    long term2 = (4 * N - 1) % MOD;
    
    long ans = (term1 * term2) % MOD;
    ans = (ans * 337) % MOD;
    
    return (int)ans;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

int killDemodogs(int n) {
    long long N = n;
    long long MOD = 1000000007;
    
    // Formula derived: n * (n+1) * (4n-1) * 337 % MOD
    long long term1 = (N * (N + 1)) % MOD;
    long long term2 = (4 * N - 1) % MOD;
    
    long long ans = (term1 * term2) % MOD;
    ans = (ans * 337) % MOD;
    
    return (int)ans;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

var killDemodogs = function(n) {
    const N = BigInt(n);
    const MOD = 1000000007n;
    
    // Formula derived: n * (n+1) * (4n-1) * 337 % MOD
    let term1 = (N * (N + 1n)) % MOD;
    let term2 = (4n * N - 1n) % MOD;
    
    let ans = (term1 * term2) % MOD;
    ans = (ans * 337n) % MOD;
    
    return Number(ans);
};

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def killDemodogs(self, n: int) -> int:
    MOD = 10**9 + 7
    # Formula derived: n * (n+1) * (4n-1) * 337 % MOD
    
    term1 = (n * (n + 1)) % MOD
    term2 = (4 * n - 1) % MOD
    
    ans = (term1 * term2) % MOD
    ans = (ans * 337) % MOD
    
    return ans

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  