## CPP

### SOLUTION

vector<vector<long long>> multiply(const vector<vector<long long>>& A,
                                   const vector<vector<long long>>& B,
                                   int n) {
    long long INF = (long long)4e18;
    vector<vector<long long>> C(n, vector<long long>(n, INF));

    for (int i = 0; i < n; i++) {
        for (int k = 0; k < n; k++) {
            if (A[i][k] == INF) continue;
            for (int j = 0; j < n; j++) {
                if (B[k][j] == INF) continue;
                long long sum = A[i][k] + B[k][j];
                if (sum < C[i][j]) C[i][j] = sum;
            }
        }
    }
    return C;
}

vector<vector<long long>> power(vector<vector<long long>> A,
                                long long p,
                                int n) {
    long long INF = (long long)4e18;
    vector<vector<long long>> res(n, vector<long long>(n, INF));

    for (int i = 0; i < n; i++) res[i][i] = 0;

    while (p > 0) {
        if (p & 1LL) res = multiply(res, A, n);
        A = multiply(A, A, n);
        p >>= 1LL;
    }
    return res;
}

long long minPathCost(int n, int m, long long k, const vector<vector<int>>& edges) {
    long long INF = (long long)4e18;
    vector<vector<long long>> adj(n, vector<long long>(n, INF));

    for (auto &e : edges) {
        int u = e[0] - 1;
        int v = e[1] - 1;
        long long w = e[2];
        if (w < adj[u][v]) adj[u][v] = w;
    }

    auto res = power(adj, k, n);
    long long ans = res[0][n - 1];

    return (ans >= INF ? -1 : ans);
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

private static long[][] multiply(long[][] A, long[][] B, int n) {
    long INF = 4_000_000_000_000_000_000L;

    long[][] C = new long[n][n];
    for (int i = 0; i < n; i++) Arrays.fill(C[i], INF);

    for (int i = 0; i < n; i++) {
        for (int k = 0; k < n; k++) {
            if (A[i][k] == INF) continue;
            for (int j = 0; j < n; j++) {
                if (B[k][j] == INF) continue;
                long sum = A[i][k] + B[k][j];
                if (sum < C[i][j]) C[i][j] = sum;
            }
        }
    }
    return C;
}

private static long[][] power(long[][] A, long p, int n) {
    long INF = 4_000_000_000_000_000_000L;

    long[][] res = new long[n][n];
    for (int i = 0; i < n; i++) {
        Arrays.fill(res[i], INF);
        res[i][i] = 0;
    }

    while (p > 0) {
        if ((p & 1) == 1) res = multiply(res, A, n);
        A = multiply(A, A, n);
        p >>= 1;
    }
    return res;
}

public static long minPathCost(int n, int m, long k, int[][] edges) {
    long INF = 4_000_000_000_000_000_000L;

    long[][] adj = new long[n][n];
    for (int i = 0; i < n; i++) Arrays.fill(adj[i], INF);

    for (int[] e : edges) {
        int u = e[0] - 1;
        int v = e[1] - 1;
        long w = e[2];
        if (w < adj[u][v]) adj[u][v] = w;
    }

    long[][] res = power(adj, k, n);
    long ans = res[0][n - 1];

    return (ans >= INF ? -1 : ans);
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  

