## CPP

### SOLUTION

int leastBricks(vector<vector<int>>& wall) {
    map<long long, int> mp;
    int n = wall.size();
    
    for(int i = 0; i < n; ++i) {
        long long sum = 0;
        // Iterate up to size - 1 to ignore the rightmost edge
        for(int j = 0; j < (wall[i].size() - 1); ++j) {
            sum += wall[i][j];
            mp[sum]++;
        }
    }
    
    int maxEdges = 0;
    for(auto const& [pos, count] : mp) {
        if(count > maxEdges) {
            maxEdges = count;
        }
    }

    return n - maxEdges;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static int leastBricks(List<List<Integer>> wall) {
    Map<Long, Integer> map = new HashMap<>();
    int n = wall.size();
    
    for (List<Integer> row : wall) {
        long sum = 0;
        // Iterate up to size - 1 to ignore the rightmost edge
        for (int i = 0; i < row.size() - 1; i++) {
            sum += row.get(i);
            map.put(sum, map.getOrDefault(sum, 0) + 1);
        }
    }
    
    int maxEdges = 0;
    for (int count : map.values()) {
        maxEdges = Math.max(maxEdges, count);
    }
    
    return n - maxEdges;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

int cmp(const void *a, const void *b) {
    long long arg1 = *(const long long *)a;
    long long arg2 = *(const long long *)b;
    if (arg1 < arg2) return -1;
    if (arg1 > arg2) return 1;
    return 0;
}

int leastBricks(int** wall, int wallSize, int* wallColSize) {
    // Collect all internal edge positions
    // Max possible edges is roughly sum of all bricks
    // We estimate a safe upper bound or realloc, but here we can calculate exact count.
    
    int totalBricks = 0;
    for(int i=0; i<wallSize; i++) totalBricks += wallColSize[i];
    
    long long* edges = (long long*)malloc(sizeof(long long) * totalBricks);
    int edgeCount = 0;
    
    for(int i=0; i<wallSize; i++) {
        long long currentSum = 0;
        for(int j=0; j < wallColSize[i] - 1; j++) {
            currentSum += wall[i][j];
            edges[edgeCount++] = currentSum;
        }
    }
    
    if (edgeCount == 0) {
        free(edges);
        return wallSize;
    }
    
    qsort(edges, edgeCount, sizeof(long long), cmp);
    
    int maxFreq = 1;
    int currentFreq = 1;
    
    for(int i=1; i<edgeCount; i++) {
        if(edges[i] == edges[i-1]) {
            currentFreq++;
        } else {
            if(currentFreq > maxFreq) maxFreq = currentFreq;
            currentFreq = 1;
        }
    }
    if(currentFreq > maxFreq) maxFreq = currentFreq;
    
    free(edges);
    return wallSize - maxFreq;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function leastBricks(wall) {
    let map = new Map();
    let n = wall.length;
    
    for (let i = 0; i < n; i++) {
        let sum = 0;
        // Iterate up to size - 1 to ignore the rightmost edge
        for (let j = 0; j < wall[i].length - 1; j++) {
            sum += wall[i][j];
            map.set(sum, (map.get(sum) || 0) + 1);
        }
    }
    
    let maxEdges = 0;
    for (let count of map.values()) {
        maxEdges = Math.max(maxEdges, count);
    }
    
    return n - maxEdges;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def leastBricks(wall: list) -> int:
    edge_counts = defaultdict(int)
    n = len(wall)
    
    for row in wall:
        current_sum = 0
        # Iterate up to size - 1 to ignore the rightmost edge
        for i in range(len(row) - 1):
            current_sum += row[i]
            edge_counts[current_sum] += 1
            
    max_edges = 0
    if edge_counts:
        max_edges = max(edge_counts.values())
        
    return n - max_edges

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  