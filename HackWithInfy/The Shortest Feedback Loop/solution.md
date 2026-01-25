## CPP

### SOLUTION

int findGirth(int n, int m, const vector<vector<int>>& edges) {
    int INF = 1e9;
    vector<vector<int>> adj(n + 1);
    for (const auto& edge : edges) {
        adj[edge[0]].push_back(edge[1]);
        adj[edge[1]].push_back(edge[0]);
    }

    int min_cycle = INF;

    for (int start_node = 1; start_node <= n; ++start_node) {
        vector<int> dist(n + 1, -1);
        vector<int> parent(n + 1, -1);
        queue<int> q;

        dist[start_node] = 0;
        q.push(start_node);

        while (!q.empty()) {
            int u = q.front();
            q.pop();

            for (int v : adj[u]) {
                if (dist[v] == -1) {
                    dist[v] = dist[u] + 1;
                    parent[v] = u;
                    q.push(v);
                } 
                else if (parent[u] != v) {
                    min_cycle = min(min_cycle, dist[u] + dist[v] + 1);
                }
            }
        }
    }

    return (min_cycle == INF ? -1 : min_cycle);
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static int findGirth(int n, int m, int[][] edges) {
    final int INF = 1_000_000_000;

    List<List<Integer>> adj = new ArrayList<>();
    for (int i = 0; i <= n; i++) {
        adj.add(new ArrayList<>());
    }

    for (int[] e : edges) {
        adj.get(e[0]).add(e[1]);
        adj.get(e[1]).add(e[0]);
    }

    int minCycle = INF;

    for (int start = 1; start <= n; start++) {
        int[] dist = new int[n + 1];
        int[] parent = new int[n + 1];
        Arrays.fill(dist, -1);
        Arrays.fill(parent, -1);

        Queue<Integer> q = new ArrayDeque<>();
        dist[start] = 0;
        q.add(start);

        while (!q.isEmpty()) {
            int u = q.poll();

            for (int v : adj.get(u)) {
                if (dist[v] == -1) {
                    dist[v] = dist[u] + 1;
                    parent[v] = u;
                    q.add(v);
                } 
                else if (parent[u] != v && parent[v] != u && dist[v] < dist[u]) {
                    minCycle = Math.min(minCycle, dist[u] + dist[v] + 1);
                }
            }
        }
    }

    return (minCycle == INF) ? -1 : minCycle;
}




### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


