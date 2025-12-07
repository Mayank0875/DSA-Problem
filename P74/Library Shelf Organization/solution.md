## CPP

### SOLUTION

int maxMatching(int n, const vector<vector<int>>& edges) {
    vector<vector<int>> tree(n + 1);
    for (const auto& edge : edges) {
        tree[edge[0]].push_back(edge[1]);
        tree[edge[1]].push_back(edge[0]);
    }

    vector<vector<int>> dp(n + 1, vector<int>(2, 0));

    function<void(int, int)> dfs = [&](int node, int par) {
        for (int child : tree[node]) {
            if (child == par) continue;
            dfs(child, node);
            dp[node][0] += dp[child][1]; 
        }
        for (int child : tree[node]) {
            if (child == par) continue;
            dp[node][1] = max(dp[node][1], dp[node][0] - dp[child][1] + dp[child][0] + 1);
        }
        dp[node][1] = max(dp[node][1], dp[node][0]);
    };

    dfs(1, -1);
    return max(dp[1][0], dp[1][1]);
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static int maxMatching(int n, int[][] edges) {
    List<List<Integer>> tree = new ArrayList<>();
    for (int i = 0; i <= n; i++) {
        tree.add(new ArrayList<>());
    }
    for (int[] edge : edges) {
        tree.get(edge[0]).add(edge[1]);
        tree.get(edge[1]).add(edge[0]);
    }

    int[][] dp = new int[n + 1][2];
    dfs(1, -1, tree, dp);

    return Math.max(dp[1][0], dp[1][1]);
}

private static void dfs(int node, int par, List<List<Integer>> tree, int[][] dp) {
    for (int child : tree.get(node)) {
        if (child == par) continue;
        dfs(child, node, tree, dp);
        dp[node][0] += dp[child][1];
    }

    for (int child : tree.get(node)) {
        if (child == par) continue;
        dp[node][1] = Math.max(dp[node][1], dp[node][0] - dp[child][1] + dp[child][0] + 1);
    }
    // Ensure dp[node][1] holds the max value for the subtree
    dp[node][1] = Math.max(dp[node][1], dp[node][0]);
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  

