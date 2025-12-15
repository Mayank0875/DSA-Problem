## CPP

### SOLUTION

struct Edge {
    int to;
    int rev;
    int cap;
    int flow;
};

void add_edge(vector<vector<Edge>> &adj, int u, int v, int cap) {
    Edge a = {v, (int)adj[v].size(), cap, 0};
    Edge b = {u, (int)adj[u].size(), 0, 0};
    adj[u].push_back(a);
    adj[v].push_back(b);
}

int bfs(int s, int t,
        vector<vector<Edge>> &adj,
        vector<pair<int,int>> &parent) {

    fill(parent.begin(), parent.end(), make_pair(-1, -1));
    parent[s] = {-2, -2};

    queue<pair<int,int>> q;
    q.push({s, INT_MAX});

    while (!q.empty()) {
        auto [u, flow] = q.front();
        q.pop();

        for (int i = 0; i < adj[u].size(); i++) {
            Edge &e = adj[u][i];
            if (parent[e.to].first == -1 && e.cap > e.flow) {
                parent[e.to] = {u, i};
                int new_flow = min(flow, e.cap - e.flow);

                if (e.to == t)
                    return new_flow;

                q.push({e.to, new_flow});
            }
        }
    }
    return 0;
}

int solve(int n, int m, const vector<pair<int,int>> &pairs) {
    int s = 0;
    int t = n + m + 1;

    vector<vector<Edge>> adj(t + 1);
    vector<pair<int,int>> parent(t + 1);

    // Source → Pilots
    for (int i = 1; i <= n; i++) {
        add_edge(adj, s, i, 1);
    }

    // Pilots → Droids
    for (auto &p : pairs) {
        add_edge(adj, p.first, n + p.second, 1);
    }

    // Droids → Sink
    for (int i = 1; i <= m; i++) {
        add_edge(adj, n + i, t, 1);
    }

    int max_flow = 0;
    int path_flow;

    while ((path_flow = bfs(s, t, adj, parent))) {
        max_flow += path_flow;

        int cur = t;
        while (cur != s) {
            int prev = parent[cur].first;
            int idx  = parent[cur].second;

            adj[prev][idx].flow += path_flow;
            int rev_idx = adj[prev][idx].rev;
            adj[cur][rev_idx].flow -= path_flow;

            cur = prev;
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


static class Edge {
    int to, rev, cap, flow;
    Edge(int to, int rev, int cap) {
        this.to = to;
        this.rev = rev;
        this.cap = cap;
        this.flow = 0;
    }
}

public static int solve(int n, int m, int[][] pairs) {
    int s = 0;
    int t = n + m + 1;
    List<List<Edge>> adj = new ArrayList<>();
    for (int i = 0; i <= t; i++) adj.add(new ArrayList<>());

    // Source to Pilots
    for (int i = 1; i <= n; i++) {
        Edge a = new Edge(i, adj.get(i).size(), 1);
        Edge b = new Edge(s, adj.get(s).size(), 0);
        adj.get(s).add(a);
        adj.get(i).add(b);
    }

    // Pilots to Droids
    for (int[] p : pairs) {
        int u = p[0];
        int v = n + p[1];
        Edge a = new Edge(v, adj.get(v).size(), 1);
        Edge b = new Edge(u, adj.get(u).size(), 0);
        adj.get(u).add(a);
        adj.get(v).add(b);
    }

    // Droids to Sink
    for (int i = 1; i <= m; i++) {
        int u = n + i;
        Edge a = new Edge(t, adj.get(t).size(), 1);
        Edge b = new Edge(u, adj.get(u).size(), 0);
        adj.get(u).add(a);
        adj.get(t).add(b);
    }

    int maxFlow = 0;
    while (true) {
        int[] parentNode = new int[t + 1];
        int[] parentEdgeIdx = new int[t + 1];
        Arrays.fill(parentNode, -1);
        Queue<Integer> q = new LinkedList<>();
        q.add(s);
        parentNode[s] = -2;

        while (!q.isEmpty()) {
            int u = q.poll();
            if (u == t) break;
            for (int i = 0; i < adj.get(u).size(); i++) {
                Edge e = adj.get(u).get(i);
                if (parentNode[e.to] == -1 && e.cap > e.flow) {
                    parentNode[e.to] = u;
                    parentEdgeIdx[e.to] = i;
                    q.add(e.to);
                }
            }
        }

        if (parentNode[t] == -1) break;

        int pathFlow = 1;
        maxFlow += pathFlow;

        int curr = t;
        while (curr != s) {
            int prev = parentNode[curr];
            int idx = parentEdgeIdx[curr];
            Edge e = adj.get(prev).get(idx);
            e.flow += pathFlow;
            adj.get(curr).get(e.rev).flow -= pathFlow;
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

