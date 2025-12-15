## CPP

### SOLUTION

vector<vector<long long>> mul(const vector<vector<long long>>& A,
                              const vector<vector<long long>>& B,
                              int n)
{
    const long long MOD = 1000000007;
    vector<vector<long long>> C(n, vector<long long>(n, 0));

    for (int i = 0; i < n; i++) {
        for (int k = 0; k < n; k++) {
            for (int j = 0; j < n; j++) {
                C[i][j] = (C[i][j] + A[i][k] * B[k][j]) % MOD;
            }
        }
    }
    return C;
}

vector<vector<long long>> modpow(vector<vector<long long>> A,
                                 long long p,
                                 int n)
{
    const long long MOD = 1000000007;
    vector<vector<long long>> res(n, vector<long long>(n, 0));

    for (int i = 0; i < n; i++) res[i][i] = 1;

    while (p > 0) {
        if (p & 1)
            res = mul(res, A, n);
        A = mul(A, A, n);
        p >>= 1;
    }
    return res;
}

int countPaths(int n, int m, long long k, const vector<vector<int>>& edges)
{
    const long long MOD = 1000000007;
    vector<vector<long long>> adj(n, vector<long long>(n, 0));

    for (const auto& edge : edges) {
        adj[edge[0] - 1][edge[1] - 1]++;
    }

    auto res = modpow(adj, k, n);
    return res[0][n - 1] % MOD;
}



### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

private static long[][] multiply(long[][] A, long[][] B, int n) {
    long[][] C = new long[n][n];
    for (int i = 0; i < n; i++) {
        for (int k = 0; k < n; k++) {
            for (int j = 0; j < n; j++) {
                C[i][j] = (C[i][j] + A[i][k] * B[k][j]) % 1000000007;
            }
        }
    }
    return C;
}

private static long[][] power(long[][] A, long p, int n) {
    long[][] res = new long[n][n];
    for (int i = 0; i < n; i++) res[i][i] = 1;

    while (p > 0) {
        if ((p & 1) == 1)
            res = multiply(res, A, n);
        A = multiply(A, A, n);
        p >>= 1;
    }
    return res;
}

public static int countPaths(int n, int m, long k, int[][] edges) {
    long[][] adj = new long[n][n];

    for (int[] edge : edges) {
        adj[edge[0] - 1][edge[1] - 1]++;
    }

    long[][] res = power(adj, k, n);
    return (int) (res[0][n - 1] % 1000000007);
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  
