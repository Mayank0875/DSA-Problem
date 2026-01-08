## CPP

### SOLUTION

typedef long long ll;
const int MOD = 1e9 + 7;

vector<vector<ll>> multiply(const vector<vector<ll>>& A, const vector<vector<ll>>& B) {
    vector<vector<ll>> C(2, vector<ll>(2));
    for (int i = 0; i < 2; i++) {
        for (int j = 0; j < 2; j++) {
            for (int k = 0; k < 2; k++) {
                C[i][j] = (C[i][j] + A[i][k] * B[k][j]) % MOD;
            }
        }
    }
    return C;
}

vector<vector<ll>> power(vector<vector<ll>> A, long long p) {
    vector<vector<ll>> res(2, vector<ll>(2));
    res[0][0] = 1; res[1][1] = 1; // Identity matrix
    while (p > 0) {
        if (p & 1) res = multiply(res, A);
        A = multiply(A, A);
        p >>= 1;
    }
    return res;
}

int countWays(long long n) {
    if (n == 1) return 1;
    if (n == 2) return 2;
    
    vector<vector<ll>> T = {{1, 1}, {1, 0}};
    
    T = power(T, n - 2);
    
    ll ans = (T[0][0] * 2 + T[0][1] * 1) % MOD;
    return ans;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static int countWays(long n) {
    if (n == 1) return 1;
    if (n == 2) return 2;
    
    long MOD = 1000000007L;
    
    long[][] T = {{1, 1}, {1, 0}};
    T = power(T, n - 2, MOD);
    
    // F(n) = T[0][0]*F(2) + T[0][1]*F(1)
    // F(2) = 2, F(1) = 1
    long ans = (T[0][0] * 2 + T[0][1] * 1) % MOD;
    return (int) ans;
}

private static long[][] multiply(long[][] A, long[][] B, long MOD) {
    long[][] C = new long[2][2];
    for (int i = 0; i < 2; i++) {
        for (int j = 0; j < 2; j++) {
            for (int k = 0; k < 2; k++) {
                C[i][j] = (C[i][j] + A[i][k] * B[k][j]) % MOD;
            }
        }
    }
    return C;
}

private static long[][] power(long[][] A, long p, long MOD) {
    long[][] res = {{1, 0}, {0, 1}};
    while (p > 0) {
        if ((p & 1) == 1) res = multiply(res, A, MOD);
        A = multiply(A, A, MOD);
        p >>= 1;
    }
    return res;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION


#define MOD 1000000007

void multiply(long long A[2][2], long long B[2][2], long long C[2][2]) {
    for (int i = 0; i < 2; i++) {
        for (int j = 0; j < 2; j++) {
            C[i][j] = 0;
            for (int k = 0; k < 2; k++) {
                C[i][j] = (C[i][j] + A[i][k] * B[k][j]) % MOD;
            }
        }
    }
}

void power(long long A[2][2], long long p, long long res[2][2]) {
    res[0][0] = 1; res[0][1] = 0;
    res[1][0] = 0; res[1][1] = 1;
    
    long long base[2][2];
    long long temp[2][2];
    
    base[0][0] = A[0][0]; base[0][1] = A[0][1];
    base[1][0] = A[1][0]; base[1][1] = A[1][1];
    
    while (p > 0) {
        if (p & 1) {
            multiply(res, base, temp);
            res[0][0] = temp[0][0]; res[0][1] = temp[0][1];
            res[1][0] = temp[1][0]; res[1][1] = temp[1][1];
        }
        multiply(base, base, temp);
        base[0][0] = temp[0][0]; base[0][1] = temp[0][1];
        base[1][0] = temp[1][0]; base[1][1] = temp[1][1];
        p >>= 1;
    }
}

int countWays(long long n) {
    if (n == 1) return 1;
    if (n == 2) return 2;
    
    long long T[2][2] = {{1, 1}, {1, 0}};
    long long res[2][2];
    
    power(T, n - 2, res);
    
    // ans = res[0][0]*2 + res[0][1]*1
    long long ans = (res[0][0] * 2 + res[0][1] * 1) % MOD;
    return (int)ans;
}
### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

const MOD = 1000000007n;

function multiply(A, B) {
    let C = [[0n, 0n], [0n, 0n]];
    for (let i = 0; i < 2; i++) {
        for (let j = 0; j < 2; j++) {
            for (let k = 0; k < 2; k++) {
                C[i][j] = (C[i][j] + A[i][k] * B[k][j]) % MOD;
            }
        }
    }
    return C;
}

function power(A, p) {
    let res = [[1n, 0n], [0n, 1n]];
    while (p > 0n) {
        if (p & 1n) res = multiply(res, A);
        A = multiply(A, A);
        p >>= 1n;
    }
    return res;
}

function countWays(n) {
    let N = BigInt(n);
    if (N === 1n) return 1;
    if (N === 2n) return 2;
    
    let T = [[1n, 1n], [1n, 0n]];
    let res = power(T, N - 2n);
    
    let ans = (res[0][0] * 2n + res[0][1] * 1n) % MOD;
    return Number(ans);
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
    if n == 1: return 1
    if n == 2: return 2
    
    def multiply(A, B):
        C = [[0, 0], [0, 0]]
        for i in range(2):
            for j in range(2):
                for k in range(2):
                    C[i][j] = (C[i][j] + A[i][k] * B[k][j]) % MOD
        return C
    
    def power(A, p):
        res = [[1, 0], [0, 1]]
        while p > 0:
            if p % 2 == 1:
                res = multiply(res, A)
            A = multiply(A, A)
            p //= 2
        return res
        
    T = [[1, 1], [1, 0]]
    res = power(T, n - 2)
    
    # F(n) = res[0][0]*F(2) + res[0][1]*F(1)
    ans = (res[0][0] * 2 + res[0][1] * 1) % MOD
    return ans

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  