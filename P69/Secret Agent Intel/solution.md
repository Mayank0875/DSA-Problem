## CPP

### SOLUTION

long long maxDataFlow(int n, int m, const vector<vector<int>>& connections) {
    vector<vector<long long>> capacity(n, vector<long long>(n, 0));
    vector<vector<int>> adj(n);

    for (const auto& conn : connections) {
        int u = conn[0] - 1;
        int v = conn[1] - 1;
        long long c = conn[2];
        
        if (u == v) continue;

        bool exists = false;
        for(int neighbor : adj[u]) {
            if(neighbor == v) { exists = true; break; }
        }
        
        if(!exists) {
            adj[u].push_back(v);
            adj[v].push_back(u); 
        }
        
        capacity[u][v] += c; 
    }

    int source = 0;
    int sink = n - 1;
    long long flow = 0;
    vector<int> parent(n);

    auto bfs = [&]() -> bool {
        fill(parent.begin(), parent.end(), -1);
        parent[source] = -2;
        queue<pair<int, long long>> q;
        q.push({source, 2e18}); // Infinite flow initially

        while (!q.empty()) {
            int cur = q.front().first;
            long long cur_flow = q.front().second;
            q.pop();

            for (int next : adj[cur]) {
                if (parent[next] == -1 && capacity[cur][next] > 0) {
                    parent[next] = cur;
                    long long new_flow = min(cur_flow, capacity[cur][next]);
                    if (next == sink) return true;
                    q.push({next, new_flow});
                }
            }
        }
        return false;
    };

    while (bfs()) {
        long long path_flow = 2e18; 
        int curr = sink;
        while (curr != source) {
            int prev = parent[curr];
            path_flow = min(path_flow, capacity[prev][curr]);
            curr = prev;
        }
        
        flow += path_flow;
        curr = sink;
        while (curr != source) {
            int prev = parent[curr];
            capacity[prev][curr] -= path_flow;
            capacity[curr][prev] += path_flow;
            curr = prev;
        }
    }

    return flow;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static long maxDataFlow(int n, int m, int[][] connections) {
    long[][] capacity = new long[n][n];
    ArrayList<Integer>[] adj = new ArrayList[n];
    for(int i=0; i<n; i++) adj[i] = new ArrayList<>();

    for (int[] conn : connections) {
        int u = conn[0] - 1;
        int v = conn[1] - 1;
        long c = conn[2];

        if (u == v) continue;

        boolean exists = false;
        for (int neighbor : adj[u]) {
            if (neighbor == v) {
                exists = true;
                break;
            }
        }

        if (!exists) {
            adj[u].add(v);
            adj[v].add(u);
        }
        capacity[u][v] += c;
    }

    int source = 0;
    int sink = n - 1;
    long totalFlow = 0;
    int[] parent = new int[n];

    while (true) {
        Arrays.fill(parent, -1);
        Queue<Integer> q = new LinkedList<>();
        q.add(source);
        parent[source] = -2;

        while (!q.isEmpty()) {
            int cur = q.poll();
            for (int next : adj[cur]) {
                if (parent[next] == -1 && capacity[cur][next] > 0) {
                    parent[next] = cur;
                    q.add(next);
                }
            }
        }

        if (parent[sink] == -1) break;

        long pathFlow = Long.MAX_VALUE;
        int curr = sink;
        while (curr != source) {
            int prev = parent[curr];
            pathFlow = Math.min(pathFlow, capacity[prev][curr]);
            curr = prev;
        }

        totalFlow += pathFlow;
        curr = sink;
        while (curr != source) {
            int prev = parent[curr];
            capacity[prev][curr] -= pathFlow;
            capacity[curr][prev] += pathFlow;
            curr = prev;
        }
    }

    return totalFlow;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  

