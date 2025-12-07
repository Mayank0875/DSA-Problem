## CPP

### SOLUTION

long long totalKawaiiness(int n, const vector<vector<int>>& edges, long long k) {
    vector<vector<int>> adj(n + 1);
    for (const auto &e : edges) {
        // e should be of size 2: {u, v}
        int u = e[0], v = e[1];
        adj[u].push_back(v);
        adj[v].push_back(u);
    }

    vector<int> sz(n + 1, 0);
    function<void(int,int)> dfs_size = [&](int u, int p) {
        sz[u] = 1;
        for (int v : adj[u]) {
            if (v == p) continue;
            dfs_size(v, u);
            sz[u] += sz[v];
        }
    };
    dfs_size(1, 0);

    long long total_kawaiiness = 0;
    for (int u = 1; u <= n; ++u) {
        total_kawaiiness++;

        for (int v : adj[u]) {
            int component_size;
            if (sz[v] < sz[u]) component_size = sz[v];
            else component_size = n - sz[u];

            if (n - component_size >= k) {
                total_kawaiiness += component_size;
            }
        }
    }

    return total_kawaiiness;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static long totalKawaiiness(int n, List<List<Integer>> edges, long k) {
    List<List<Integer>> adj = new ArrayList<>();
    for (int i = 0; i <= n; i++) adj.add(new ArrayList<>());

    for (List<Integer> e : edges) {
        int u = e.get(0);
        int v = e.get(1);
        adj.get(u).add(v);
        adj.get(v).add(u);
    }

    int[] sz = new int[n + 1];

    java.util.function.BiConsumer<Integer, Integer> dfs = new java.util.function.BiConsumer<>() {
        @Override
        public void accept(Integer u, Integer p) {
            sz[u] = 1;
            for (int v : adj.get(u)) {
                if (v == p) continue;
                this.accept(v, u);
                sz[u] += sz[v];
            }
        }
    };

    dfs.accept(1, 0);

    long total = 0;

    for (int u = 1; u <= n; u++) {
        total++;

        for (int v : adj.get(u)) {
            int componentSize;

            if (sz[v] < sz[u]) componentSize = sz[v];
            else componentSize = n - sz[u];

            if (n - componentSize >= k) {
                total += componentSize;
            }
        }
    }

    return total;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  
