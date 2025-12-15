## CPP

### SOLUTION

struct Edge {
    int to;
    int rev;   // index of reverse edge
    int cap;
    int flow;
};

int maxDays(int n, int m, const vector<vector<int>>& teleporters) {
    vector<vector<Edge>> adj(n + 1);
    vector<int> parent_node(n + 1), parent_edge_index(n + 1);

    auto add_edge = [&](int u, int v, int cap) {
        Edge a = {v, (int)adj[v].size(), cap, 0};
        Edge b = {u, (int)adj[u].size(), 0, 0};
        adj[u].push_back(a);
        adj[v].push_back(b);
    };

    for (const auto& t : teleporters) {
        add_edge(t[0], t[1], 1);
    }

    int flow = 0;

    while (true) {
        fill(parent_node.begin(), parent_node.end(), -1);
        queue<int> q;
        q.push(1);
        parent_node[1] = 0;

        while (!q.empty()) {
            int u = q.front();
            q.pop();
            if (u == n) break;

            for (int i = 0; i < (int)adj[u].size(); i++) {
                Edge &e = adj[u][i];
                if (parent_node[e.to] == -1 && e.cap > e.flow) {
                    parent_node[e.to] = u;
                    parent_edge_index[e.to] = i;
                    q.push(e.to);
                }
            }
        }

        if (parent_node[n] == -1) break;

        int push = INT_MAX;
        int curr = n;
        while (curr != 1) {
            int p = parent_node[curr];
            int idx = parent_edge_index[curr];
            push = min(push, adj[p][idx].cap - adj[p][idx].flow);
            curr = p;
        }

        curr = n;
        while (curr != 1) {
            int p = parent_node[curr];
            int idx = parent_edge_index[curr];
            adj[p][idx].flow += push;
            int rev_idx = adj[p][idx].rev;
            adj[curr][rev_idx].flow -= push;
            curr = p;
        }

        flow += push;
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


private static class Edge {
    int to, rev, cap, flow;
    Edge(int to, int rev, int cap) {
        this.to = to;
        this.rev = rev;
        this.cap = cap;
        this.flow = 0;
    }
}

public static int maxDays(int n, int m, int[][] teleporters) {
    List<List<Edge>> adj = new ArrayList<>();
    for (int i = 0; i <= n; i++) adj.add(new ArrayList<>());

    for (int[] t : teleporters) {
        int u = t[0];
        int v = t[1];
        Edge a = new Edge(v, adj.get(v).size(), 1);
        Edge b = new Edge(u, adj.get(u).size(), 0);
        adj.get(u).add(a);
        adj.get(v).add(b);
    }

    int flow = 0;
    int[] parentNode = new int[n + 1];
    int[] parentEdgeIndex = new int[n + 1];

    while (true) {
        Arrays.fill(parentNode, -1);
        Queue<Integer> q = new LinkedList<>();
        q.offer(1);
        parentNode[1] = 0;

        while (!q.isEmpty()) {
            int u = q.poll();
            if (u == n) break;

            for (int i = 0; i < adj.get(u).size(); i++) {
                Edge e = adj.get(u).get(i);
                if (parentNode[e.to] == -1 && e.cap > e.flow) {
                    parentNode[e.to] = u;
                    parentEdgeIndex[e.to] = i;
                    q.offer(e.to);
                }
            }
        }

        if (parentNode[n] == -1) break;

        int push = Integer.MAX_VALUE;
        int curr = n;
        while (curr != 1) {
            int p = parentNode[curr];
            int idx = parentEdgeIndex[curr];
            Edge e = adj.get(p).get(idx);
            push = Math.min(push, e.cap - e.flow);
            curr = p;
        }

        curr = n;
        while (curr != 1) {
            int p = parentNode[curr];
            int idx = parentEdgeIndex[curr];
            Edge e = adj.get(p).get(idx);
            e.flow += push;
            Edge rev = adj.get(curr).get(e.rev);
            rev.flow -= push;
            curr = p;
        }

        flow += push;
    }

    return flow;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


