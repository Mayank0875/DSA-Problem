## CPP

### SOLUTION
## CPP

int countRitualPaths(int n, int m, const vector<vector<int>>& edges) {
    const int MOD = 1e9 + 7;
    vector<vector<int>> adj(n);
    for (const auto& edge : edges) {
        adj[edge[0] - 1].push_back(edge[1] - 1);
    }
    vector<vector<int>> dp(1 << n, vector<int>(n, 0));
    dp[1][0] = 1;

    for (int mask = 1; mask < (1 << n); ++mask) {
        if ((mask & (1 << (n - 1))) && mask != ((1 << n) - 1)) continue;

        for (int u = 0; u < n; ++u) {
            if ((mask >> u) & 1) {
                if (dp[mask][u] == 0) continue;

                for (int v : adj[u]) {
                    if (!((mask >> v) & 1)) {
                        int newMask = mask | (1 << v);
                        dp[newMask][v] = (dp[newMask][v] + dp[mask][u]) % MOD;
                    }
                }
            }
        }
    }

    return dp[(1 << n) - 1][n - 1];
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static int countRitualPaths(int n, int m, int[][] edges) {
    int MOD = 1000000007;
    ArrayList<Integer>[] adj = new ArrayList[n];
    for (int i = 0; i < n; i++) adj[i] = new ArrayList<>();
    
    for (int[] edge : edges) {
        adj[edge[0] - 1].add(edge[1] - 1);
    }

    int[][] dp = new int[1 << n][n];
    dp[1][0] = 1;

    for (int mask = 1; mask < (1 << n); ++mask) {
        if (((mask >> (n - 1)) & 1) == 1 && mask != ((1 << n) - 1)) continue;

        for (int u = 0; u < n; ++u) {
            if (((mask >> u) & 1) == 1) {
                if (dp[mask][u] == 0) continue;

                for (int v : adj[u]) {
                    if (((mask >> v) & 1) == 0) {
                        int newMask = mask | (1 << v);
                        dp[newMask][v] = (dp[newMask][v] + dp[mask][u]) % MOD;
                    }
                }
            }
        }
    }

    return dp[(1 << n) - 1][n - 1];
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



