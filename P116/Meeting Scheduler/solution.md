## CPP

### SOLUTION

int findLongestChain(vector<vector<int>>& pairs) {
    // Sort based on the end time (second element)
    std::sort(pairs.begin(), pairs.end(), [](const std::vector<int>& a, const std::vector<int>& b) {
        return a[1] < b[1];
    });

    if (pairs.empty()) return 0;

    std::vector<int> prev = pairs[0];
    int res = 1;

    for (size_t i = 1; i < pairs.size(); i++) {
        const std::vector<int>& cur = pairs[i];
        // If current start is strictly greater than previous end
        if (cur[0] > prev[1]) {
            res++;
            prev = cur;
        }
    }

    return res;        
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static int findLongestChain(int[][] pairs) {
    // Sort based on the end time (second element)
    Arrays.sort(pairs, (a, b) -> Integer.compare(a[1], b[1]));

    if (pairs.length == 0) return 0;

    int[] prev = pairs[0];
    int res = 1;

    for (int i = 1; i < pairs.length; i++) {
        int[] cur = pairs[i];
        if (cur[0] > prev[1]) {
            res++;
            prev = cur;
        }
    }

    return res;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

int compare(const void* a, const void* b) {
    int* pairA = *(int**)a;
    int* pairB = *(int**)b;
    return pairA[1] - pairB[1];
}

int findLongestChain(int** pairs, int pairsSize, int* pairsColSize) {
    if (pairsSize == 0) return 0;

    qsort(pairs, pairsSize, sizeof(int*), compare);

    int* prev = pairs[0];
    int res = 1;

    for (int i = 1; i < pairsSize; i++) {
        int* cur = pairs[i];
        if (cur[0] > prev[1]) {
            res++;
            prev = cur;
        }
    }

    return res;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function findLongestChain(pairs) {
    // Sort based on the end time
    pairs.sort((a, b) => a[1] - b[1]);

    if (pairs.length === 0) return 0;

    let prev = pairs[0];
    let res = 1;

    for (let i = 1; i < pairs.length; i++) {
        const cur = pairs[i];
        if (cur[0] > prev[1]) {
            res++;
            prev = cur;
        }
    }

    return res;    
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def findLongestChain(pairs: list) -> int:
    # Sort based on the end time (second element)
    pairs.sort(key=lambda x: x[1])

    if not pairs:
        return 0

    prev = pairs[0]
    res = 1

    for cur in pairs[1:]:
        if cur[0] > prev[1]:
            res += 1
            prev = cur

    return res

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  