## CPP

### SOLUTION

void dfs1(int node, const vector<vector<int>>& graph, vector<bool>& vis, stack<int>& order) {
    vis[node] = true;
    for (int child : graph[node]) {
        if (!vis[child]) {
            dfs1(child, graph, vis, order);
        }
    }
    order.push(node);
}

void dfs2(int node, const vector<vector<int>>& reverse_graph, vector<bool>& vis) {
    vis[node] = true;
    for (int child : reverse_graph[node]) {
        if (!vis[child]) {
            dfs2(child, reverse_graph, vis);
        }
    }
}

int findGuildCount(int n, int m, const vector<vector<int>>& edges) {
    vector<vector<int>> graph(n + 1), reverse_graph(n + 1);
    for (const auto& edge : edges) {
        graph[edge[0]].push_back(edge[1]);
        reverse_graph[edge[1]].push_back(edge[0]);
    }

    vector<bool> vis(n + 1, false);
    stack<int> order;

    for (int i = 1; i <= n; ++i) {
        if (!vis[i]) {
            dfs1(i, graph, vis, order);
        }
    }

    fill(vis.begin(), vis.end(), false);
    int k = 0;

    while (!order.empty()) {
        int node = order.top();
        order.pop();
        if (!vis[node]) {
            k++;
            dfs2(node, reverse_graph, vis);
        }
    }
    
    return k;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

private static void dfs1(int node, ArrayList<ArrayList<Integer>> graph, boolean[] vis, Stack<Integer> order) {
    vis[node] = true;
    for (int child : graph.get(node)) {
        if (!vis[child]) {
            dfs1(child, graph, vis, order);
        }
    }
    order.push(node);
}

private static void dfs2(int node, ArrayList<ArrayList<Integer>> reverseGraph, boolean[] vis) {
    vis[node] = true;
    for (int child : reverseGraph.get(node)) {
        if (!vis[child]) {
            dfs2(child, reverseGraph, vis);
        }
    }
}

public static int findGuildCount(int n, int m, int[][] edges) {
    ArrayList<ArrayList<Integer>> graph = new ArrayList<>();
    ArrayList<ArrayList<Integer>> reverseGraph = new ArrayList<>();
    
    for (int i = 0; i <= n; i++) {
        graph.add(new ArrayList<>());
        reverseGraph.add(new ArrayList<>());
    }

    for (int[] edge : edges) {
        graph.get(edge[0]).add(edge[1]);
        reverseGraph.get(edge[1]).add(edge[0]);
    }

    boolean[] vis = new boolean[n + 1];
    Stack<Integer> order = new Stack<>();

    for (int i = 1; i <= n; ++i) {
        if (!vis[i]) {
            dfs1(i, graph, vis, order);
        }
    }

    Arrays.fill(vis, false);
    int k = 0;

    while (!order.isEmpty()) {
        int node = order.pop();
        if (!vis[node]) {
            k++;
            dfs2(node, reverseGraph, vis);
        }
    }

    return k;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  
