## CPP

### SOLUTION

void dfs(int v, vector<vector<int>> &adj, vector<bool> &visited, vector<int> &topo_order) {
    visited[v] = true;
    for (int u : adj[v]) {
        if (!visited[u]) {
            dfs(u, adj, visited, topo_order);
        }
    }
    topo_order.push_back(v);
}

int countTimelines(int n, vector<vector<int>>& edges) {
    vector<vector<int>> adj(n + 1);
    for (auto& edge : edges) {
        adj[edge[0]].push_back(edge[1]);
    }

    vector<bool> visited(n + 1, false);
    vector<int> topo_order;
    
    for (int i = 1; i <= n; ++i) {
        if (!visited[i]) {
            dfs(i, adj, visited, topo_order);
        }
    }
    
    long long MOD = 1e9 + 7;
    vector<long long> dp(n + 1, 0);
    dp[n] = 1;

    for (int u : topo_order) {
        for (int v : adj[u]) {
            dp[u] = (dp[u] + dp[v]) % MOD;
        }
    }
    
    return dp[1];
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

private static void dfs(int v, List<List<Integer>> adj, boolean[] visited, List<Integer> topoOrder) {
    visited[v] = true;
    for (int u : adj.get(v)) {
        if (!visited[u]) {
            dfs(u, adj, visited, topoOrder);
        }
    }
    topoOrder.add(v);
}

public static int countTimelines(int n, int[][] edges) {
    List<List<Integer>> adj = new ArrayList<>();
    for (int i = 0; i <= n; i++) {
        adj.add(new ArrayList<>());
    }
    for (int[] edge : edges) {
        adj.get(edge[0]).add(edge[1]);
    }

    boolean[] visited = new boolean[n + 1];
    List<Integer> topoOrder = new ArrayList<>();

    for (int i = 1; i <= n; i++) {
        if (!visited[i]) {
            dfs(i, adj, visited, topoOrder);
        }
    }

    long mod = 1000000007L;
    long[] dp = new long[n + 1];
    dp[n] = 1;

    for (int u : topoOrder) {
        for (int v : adj.get(u)) {
            dp[u] = (dp[u] + dp[v]) % mod;
        }
    }

    return (int) dp[1];
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  
