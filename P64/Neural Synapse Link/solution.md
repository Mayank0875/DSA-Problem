## CPP

### SOLUTION

int getSquaredDistance(vector<int>& a, vector<int>& b) {
    int dx = a[0] - b[0];
    int dy = a[1] - b[1];
    return dx * dx + dy * dy;
}

int minTransmissionCost(int n, vector<vector<int>>& stations) {
    vector<int> min_dist(n, INT_MAX);
    vector<bool> visited(n, false);
    
    min_dist[0] = 0;
    int result = 0;
    
    for (int i = 0; i < n; ++i) {
        int u = -1;
        
        for (int j = 0; j < n; ++j) {
            if (!visited[j] && (u == -1 || min_dist[j] < min_dist[u])) {
                u = j;
            }
        }
        
        visited[u] = true;
        result = max(result, min_dist[u]);
        
        for (int v = 0; v < n; ++v) {
            if (!visited[v]) {
                int dist = getSquaredDistance(stations[u], stations[v]);
                if (dist < min_dist[v]) {
                    min_dist[v] = dist;
                }
            }
        }
    }
    
    return result;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static int getSquaredDistance(int[] a, int[] b) {
    int dx = a[0] - b[0];
    int dy = a[1] - b[1];
    return dx * dx + dy * dy;
}

public static int minTransmissionCost(int n, int[][] stations) {
    int[] minDist = new int[n];
    boolean[] visited = new boolean[n];
    
    Arrays.fill(minDist, Integer.MAX_VALUE);
    minDist[0] = 0;
    
    int result = 0;
    
    for (int i = 0; i < n; i++) {
        int u = -1;
        
        for (int j = 0; j < n; j++) {
            if (!visited[j] && (u == -1 || minDist[j] < minDist[u])) {
                u = j;
            }
        }
        
        visited[u] = true;
        result = Math.max(result, minDist[u]);
        
        for (int v = 0; v < n; v++) {
            if (!visited[v]) {
                int dist = getSquaredDistance(stations[u], stations[v]);
                if (dist < minDist[v]) {
                    minDist[v] = dist;
                }
            }
        }
    }
    
    return result;
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


