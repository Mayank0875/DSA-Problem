## CPP

### SOLUTION

int minStreets(int n, int m, const vector<vector<int>>& streets) {
    vector<vector<int>> capacity(n + 1, vector<int>(n + 1, 0));
    vector<vector<int>> adj(n + 1);

    for (const auto& street : streets) {
        int u = street[0];
        int v = street[1];
        // Add edges in both directions for undirected graph
        adj[u].push_back(v);
        adj[v].push_back(u);
        // Capacities are 1 (1 street = 1 unit of flow)
        capacity[u][v]++;
        capacity[v][u]++; 
    }

    int source = 1;
    int sink = n;
    int max_flow = 0;
    vector<int> parent(n + 1);

    while (true) {
        fill(parent.begin(), parent.end(), -1);
        queue<pair<int, int>> q;
        q.push({source, INT_MAX});
        parent[source] = source;

        int path_flow = 0;
        int path_end = -1;

        while (!q.empty()) {
            int u = q.front().first;
            int flow = q.front().second;
            q.pop();

            if (u == sink) {
                path_flow = flow;
                path_end = sink;
                break;
            }

            for (int v : adj[u]) {
                if (parent[v] == -1 && capacity[u][v] > 0) {
                    parent[v] = u;
                    int new_flow = min(flow, capacity[u][v]);
                    q.push({v, new_flow});
                }
            }
        }

        if (parent[sink] == -1) break; // No augmenting path

        max_flow += path_flow;
        int curr = sink;
        while (curr != source) {
            int prev = parent[curr];
            capacity[prev][curr] -= path_flow;
            capacity[curr][prev] += path_flow;
            curr = prev;
        }
    }

    return max_flow;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static int minStreets(int n, int m, int[][] streets) {
    // Local capacity matrix and adjacency list
    int[][] capacity = new int[n + 1][n + 1];
    List<List<Integer>> adj = new ArrayList<>();
    for (int i = 0; i <= n; i++) adj.add(new ArrayList<>());

    for (int[] street : streets) {
        int u = street[0];
        int v = street[1];
        adj.get(u).add(v);
        adj.get(v).add(u);
        capacity[u][v]++;
        capacity[v][u]++;
    }

    int source = 1;
    int sink = n;
    int maxFlow = 0;
    int[] parent = new int[n + 1];

    while (true) {
        Arrays.fill(parent, -1);
        Queue<Integer> q = new LinkedList<>();
        q.add(source);
        parent[source] = source;

        while (!q.isEmpty()) {
            int u = q.poll();
            if (u == sink) break;

            for (int v : adj.get(u)) {
                if (parent[v] == -1 && capacity[u][v] > 0) {
                    parent[v] = u;
                    q.add(v);
                }
            }
        }

        if (parent[sink] == -1) break;

        int pathFlow = Integer.MAX_VALUE;
        int curr = sink;
        while (curr != source) {
            int prev = parent[curr];
            pathFlow = Math.min(pathFlow, capacity[prev][curr]);
            curr = prev;
        }

        maxFlow += pathFlow;
        curr = sink;
        while (curr != source) {
            int prev = parent[curr];
            capacity[prev][curr] -= pathFlow;
            capacity[curr][prev] += pathFlow;
            curr = prev;
        }
    }

    return maxFlow;
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


