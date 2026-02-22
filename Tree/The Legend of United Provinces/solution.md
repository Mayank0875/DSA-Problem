## CPP

### SOLUTION


int solve(vector<vector<int>>& isConnected) {
    int n = isConnected.size();
    vector<bool> visited(n, false);
    int provinces = 0;

    for (int i = 0; i < n; i++) {
        if (visited[i]) continue;

        queue<int> q;
        q.push(i);
        visited[i] = true;

        while (!q.empty()) {
            int city = q.front();
            q.pop();

            for (int j = 0; j < n; j++) {
                if (isConnected[city][j] == 1 && !visited[j]) {
                    visited[j] = true;
                    q.push(j);
                }
            }
        }
        provinces++;
    }
    return provinces;
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION


public static int solve(int[][] isConnected) {
    int n = isConnected.length;
    boolean[] visited = new boolean[n];
    int provinces = 0;

    for (int i = 0; i < n; i++) {
        if (!visited[i]) {
            Queue<Integer> q = new LinkedList<>();
            q.add(i);
            visited[i] = true;
            while (!q.isEmpty()) {
                int city = q.poll();
                for (int j = 0; j < n; j++) {
                    if (isConnected[city][j] == 1 && !visited[j]) {
                        visited[j] = true;
                        q.add(j);
                    }
                }
            }
            provinces++;
        }
    }
    return provinces;
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVASCRIPT

### SOLUTION


function solve(isConnected) {
    const n = isConnected.length;
    const visited = new Array(n).fill(false);
    let provinces = 0;

    for (let i = 0; i < n; i++) {
        if (!visited[i]) {
            const queue = [i];
            visited[i] = true;
            while (queue.length > 0) {
                const city = queue.shift();
                for (let j = 0; j < n; j++) {
                    if (isConnected[city][j] === 1 && !visited[j]) {
                        visited[j] = true;
                        queue.push(j);
                    }
                }
            }
            provinces++;
        }
    }
    return provinces;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def solve(isConnected: list[list[int]]) -> int:
    n = len(isConnected)
    visited = [False] * n
    provinces = 0
    
    for i in range(n):
        if not visited[i]:
            queue = deque([i])
            visited[i] = True
            while queue:
                city = queue.popleft()
                for j in range(n):
                    if isConnected[city][j] == 1 and not visited[j]:
                        visited[j] = True
                        queue.append(j)
            provinces += 1
    return provinces

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  