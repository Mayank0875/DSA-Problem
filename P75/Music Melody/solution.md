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
        queue<int> q;

        dist[start_node] = 0;
        q.push(start_node);

        while (!q.empty()) {
            int u = q.front();
            q.pop();

            for (int v : adj[u]) {
                if (dist[v] == -1) {
                    // Not visited yet
                    dist[v] = dist[u] + 1;
                    q.push(v);
                } else if (dist[v] >= dist[u]) {
                    // Visited and not the parent (since dist[v] >= dist[u], v cannot be the parent of u in BFS tree)
                    // We found a cycle. The length is dist[u] + dist[v] + 1
                    min_cycle = min(min_cycle, dist[u] + dist[v] + 1);
                }
            }
        }
    }

    if (min_cycle == INF) return -1;
    return min_cycle;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static int findGirth(int n, int m, int[][] edges) {
    int INF = 1000000000;
    List<List<Integer>> adj = new ArrayList<>();
    for (int i = 0; i <= n; i++) {
        adj.add(new ArrayList<>());
    }

    for (int[] edge : edges) {
        adj.get(edge[0]).add(edge[1]);
        adj.get(edge[1]).add(edge[0]);
    }

    int minCycle = INF;

    // BFS from each node
    for (int startNode = 1; startNode <= n; startNode++) {
        int[] dist = new int[n + 1];
        Arrays.fill(dist, -1);
        Queue<Integer> queue = new LinkedList<>();

        dist[startNode] = 0;
        queue.add(startNode);

        while (!queue.isEmpty()) {
            int u = queue.poll();

            for (int v : adj.get(u)) {
                if (dist[v] == -1) {
                    dist[v] = dist[u] + 1;
                    queue.add(v);
                } else if (dist[v] >= dist[u]) {
                    // Found a cycle
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


