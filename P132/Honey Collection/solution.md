## CPP

### SOLUTION

int minReorder(int n, vector<vector<int>>& connections) {
    vector<vector<int>> adj(n + 1);
    for (const auto& edge : connections) {
        adj[edge[0]].push_back(edge[1]);
        adj[edge[1]].push_back(-edge[0]);
    }

    int correctDirectionCount = 0;
    vector<int> stack;
    vector<bool> visited(n + 1, false);
    
    stack.push_back(1);
    visited[1] = true;
    
    while (!stack.empty()) {
        int u = stack.back();
        stack.pop_back();
        
        for (int neighbor : adj[u]) {
            int v = abs(neighbor);
            if (!visited[v]) {
                visited[v] = true;
                if (neighbor < 0) {
                    correctDirectionCount++;
                }
                stack.push_back(v);
            }
        }
    }
    
    return (n - 1) - correctDirectionCount;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static int minReorder(int n, int[][] connections) {
    ArrayList<ArrayList<Integer>> adj = new ArrayList<>();
    for (int i = 0; i <= n; i++) adj.add(new ArrayList<>());
    
    for (int[] edge : connections) {
        adj.get(edge[0]).add(edge[1]);       // Positive: u -> v
        adj.get(edge[1]).add(-edge[0]);      // Negative: v -> u
    }
    
    int correctDirectionCount = 0;
    boolean[] visited = new boolean[n + 1];
    java.util.Stack<Integer> stack = new java.util.Stack<>();
    
    stack.push(1);
    visited[1] = true;
    
    while (!stack.isEmpty()) {
        int u = stack.pop();
        
        for (int neighbor : adj.get(u)) {
            int v = Math.abs(neighbor);
            if (!visited[v]) {
                visited[v] = true;
                // neighbor < 0 means original edge was v -> u (towards root)
                if (neighbor < 0) {
                    correctDirectionCount++;
                }
                stack.push(v);
            }
        }
    }
    
    return (n - 1) - correctDirectionCount;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

// Structure for Adjacency List Node
typedef struct Node {
    int val; // Positive for forward, negative for backward
    struct Node* next;
} Node;

int minReorder(int n, int** connections, int connectionsSize, int* connectionsColSize) {
    Node** adj = (Node**)calloc(n + 1, sizeof(Node*));
    
    for (int i = 0; i < connectionsSize; i++) {
        int u = connections[i][0];
        int v = connections[i][1];
        
        // Add u -> v (positive)
        Node* newNode1 = (Node*)malloc(sizeof(Node));
        newNode1->val = v;
        newNode1->next = adj[u];
        adj[u] = newNode1;
        
        // Add v -> u (negative to mark reverse)
        Node* newNode2 = (Node*)malloc(sizeof(Node));
        newNode2->val = -u;
        newNode2->next = adj[v];
        adj[v] = newNode2;
    }
    
    int correctDirectionCount = 0;
    int* queue = (int*)malloc((n + 1) * sizeof(int));
    int* visited = (int*)calloc(n + 1, sizeof(int));
    int front = 0, rear = 0;
    
    // BFS
    queue[rear++] = 1;
    visited[1] = 1;
    
    while (front < rear) {
        int u = queue[front++];
        Node* curr = adj[u];
        while (curr != NULL) {
            int neighbor = curr->val;
            int v = abs(neighbor);
            
            if (!visited[v]) {
                visited[v] = 1;
                // If negative, it points towards root (correct)
                if (neighbor < 0) {
                    correctDirectionCount++;
                }
                queue[rear++] = v;
            }
            curr = curr->next;
        }
    }
    
    // Cleanup
    for (int i = 0; i <= n; i++) {
        Node* curr = adj[i];
        while (curr) {
            Node* temp = curr;
            curr = curr->next;
            free(temp);
        }
    }
    free(adj);
    free(queue);
    free(visited);
    
    return (n - 1) - correctDirectionCount;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function minReorder(n, connections) {
    let adj = Array.from({ length: n + 1 }, () => []);
    
    for (let [u, v] of connections) {
        adj[u].push(v);       // Positive: original u -> v
        adj[v].push(-u);      // Negative: original v -> u
    }
    
    let correctDirectionCount = 0;
    let visited = new Uint8Array(n + 1);
    let stack = [1];
    visited[1] = 1;
    
    while (stack.length > 0) {
        let u = stack.pop();
        
        for (let neighbor of adj[u]) {
            let v = Math.abs(neighbor);
            if (visited[v] === 0) {
                visited[v] = 1;
                // neighbor < 0 means v -> u (points to root), which is correct
                if (neighbor < 0) {
                    correctDirectionCount++;
                }
                stack.push(v);
            }
        }
    }
    
    return (n - 1) - correctDirectionCount;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def minReorder(n: int, connections: list) -> int:
    adj = [[] for _ in range(n + 1)]
    for u, v in connections:
        adj[u].append(v)      # Positive: u -> v
        adj[v].append(-u)     # Negative: v -> u
        
    correct_direction_count = 0
    visited = [False] * (n + 1)
    stack = [1]
    visited[1] = True
    
    while stack:
        u = stack.pop()
        for neighbor in adj[u]:
            v = abs(neighbor)
            if not visited[v]:
                visited[v] = True
                # neighbor < 0 means v -> u (towards root), which is correct
                if neighbor < 0:
                    correct_direction_count += 1
                stack.append(v)
                
    return (n - 1) - correct_direction_count


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  