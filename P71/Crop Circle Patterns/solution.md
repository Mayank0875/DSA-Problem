## CPP

### SOLUTION

pair<int, int> solveTradeRings(int n, vector<int>& a) {
    vector<set<int>> adj(n + 1);
    for (int i = 0; i < n; ++i) {
        int u = i + 1;
        int v = a[i];
        adj[u].insert(v);
        adj[v].insert(u);
    }

    vector<int> vis(n + 1, 0);
    int start = 0;          
    int cycles = 0;          
    int flag = 0;            

    function<void(int,int)> dfs = [&](int u, int parent) {
        vis[u] = start;
        for (int v : adj[u]) {
            if (!vis[v]) {
                dfs(v, u);
            } else if (v != parent) {
                flag = 1; 
            }
        }
    };

    for (int i = 1; i <= n; i++) {
        if (!vis[i]) {
            start++;        
            dfs(i, -1);
            cycles += flag; 
            flag = 0;       
        }
    }

    int components = start;
    int min_rings = min(components, cycles + 1);
    int max_rings = components;


    return {min_rings, max_rings};
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static int[] solveTradeRings(int n, int[] a) {

    // adjacency as HashSet (same as set<int> in C++)
    List<Set<Integer>> adj = new ArrayList<>();
    for (int i = 0; i <= n; i++) {
        adj.add(new HashSet<>());
    }

    // build graph
    for (int i = 0; i < n; i++) {
        int u = i + 1;
        int v = a[i];
        adj.get(u).add(v);
        adj.get(v).add(u);
    }

    int[] vis = new int[n + 1];
    int start = 0;       // number of components
    int cycles = 0;      // components that contain a cycle
    final int[] flag = {0}; // used inside DFS lambda

    // DFS (u, parent)
    class DFS {
        void run(int u, int parent) {
            vis[u] = start;
            for (int v : adj.get(u)) {
                if (vis[v] == 0) { 
                    run(v, u);
                } else if (v != parent) { 
                    flag[0] = 1;   // back-edge → cycle found
                }
            }
        }
    }
    DFS dfs = new DFS();

    // iterate over components
    for (int i = 1; i <= n; i++) {
        if (vis[i] == 0) {
            start++;
            dfs.run(i, -1);
            cycles += flag[0];
            flag[0] = 0;
        }
    }

    int components = start;
    int minRings = Math.min(components, cycles + 1);
    int maxRings = components;

    return new int[]{minRings, maxRings};
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  

