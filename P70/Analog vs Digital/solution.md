## CPP

### SOLUTION

int bfs(int n, const vector<vector<int>>& adj) {
    vector<int> dist(n + 1, -1);
    queue<int> q;

    dist[1] = 0;
    q.push(1);

    while (!q.empty()) {
        int u = q.front();
        q.pop();

        if (u == n) return dist[n];

        for (int v : adj[u]) {
            if (dist[v] == -1) {
                dist[v] = dist[u] + 1;
                q.push(v);
            }
        }
    }
    return -1;
}

int solve(int n, int m, vector<vector<int>> edges) {
    vector<vector<int>> adj1(n + 1);
    vector<vector<bool>> hasEdge(n + 1, vector<bool>(n + 1, false));

    for (auto& edge : edges) {
        adj1[edge[0]].push_back(edge[1]);
        adj1[edge[1]].push_back(edge[0]);
        hasEdge[edge[0]][edge[1]] = true;
        hasEdge[edge[1]][edge[0]] = true;
    }
    vector<vector<int>> adj2(n + 1);
    for (int i = 1; i <= n; ++i) {
        for (int j = i + 1; j <= n; ++j) {
            if (!hasEdge[i][j]) {
                adj2[i].push_back(j);
                adj2[j].push_back(i);
            }
        }
    }

    int dist1 = bfs(n, adj1);
    int dist2 = bfs(n, adj2);

    if (dist1 == -1 || dist2 == -1) return -1;
    return max(dist1, dist2);
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

private static int bfs(int n, List<List<Integer>> adj) {
    int[] dist = new int[n + 1];
    Arrays.fill(dist, -1);
    Queue<Integer> q = new LinkedList<>();

    dist[1] = 0;
    q.add(1);

    while (!q.isEmpty()) {
        int u = q.poll();
        if (u == n) return dist[n];

        for (int v : adj.get(u)) {
            if (dist[v] == -1) {
                dist[v] = dist[u] + 1;
                q.add(v);
            }
        }
    }
    return -1;
}

public static int solve(int n, int m, int[][] edges) {
    List<List<Integer>> adj1 = new ArrayList<>();
    boolean[][] hasEdge = new boolean[n + 1][n + 1];

    for (int i = 0; i <= n; i++) {
        adj1.add(new ArrayList<>());
    }

    for (int[] edge : edges) {
        adj1.get(edge[0]).add(edge[1]);
        adj1.get(edge[1]).add(edge[0]);
        hasEdge[edge[0]][edge[1]] = true;
        hasEdge[edge[1]][edge[0]] = true;
    }

    List<List<Integer>> adj2 = new ArrayList<>();
    for (int i = 0; i <= n; i++) {
        adj2.add(new ArrayList<>());
    }

    for (int i = 1; i <= n; i++) {
        for (int j = i + 1; j <= n; j++) {
            if (!hasEdge[i][j]) {
                adj2.get(i).add(j);
                adj2.get(j).add(i);
            }
        }
    }

    int dist1 = bfs(n, adj1);
    int dist2 = bfs(n, adj2);

    if (dist1 == -1 || dist2 == -1) return -1;
    return Math.max(dist1, dist2);
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  

