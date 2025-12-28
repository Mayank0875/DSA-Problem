## CPP

### SOLUTION

int maxValue(vector<int>& canisters) {
    sort(canisters.begin(), canisters.end());
    int ans = 0;
    int n = canisters.size();
    // We start from index n/3 and pick every second element
    for (int i = n / 3; i < n; i += 2) {
        ans += canisters[i];
    }
    return ans;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static int maxValue(int[] canisters) {
    Arrays.sort(canisters);
    int ans = 0;
    int n = canisters.length;
    // We start from index n/3 and pick every second element
    for (int i = n / 3; i < n; i += 2) {
        ans += canisters[i];
    }
    return ans;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

int compare(const void* a, const void* b) {
    return (*(int*)a - *(int*)b);
}

int maxValue(int* canisters, int canistersSize) {
    qsort(canisters, canistersSize, sizeof(int), compare);
    int ans = 0;
    // We start from index n/3 and pick every second element
    for (int i = canistersSize / 3; i < canistersSize; i += 2) {
        ans += canisters[i];
    }
    return ans;
}
### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function maxValue(canisters) {
    // Default sort in JS is lexicographical, so we need a numeric comparator
    canisters.sort((a, b) => a - b);
    let ans = 0;
    const n = canisters.length;
    // We start from index n/3 and pick every second element
    for (let i = n / 3; i < n; i += 2) {
        ans += canisters[i];
    }
    return ans;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def maxvalue(canisters: list) -> int:
    canisters.sort()
    ans = 0
    n = len(canisters)
    # We start from index n/3 and pick every second element
    for i in range(n // 3, n, 2):
        ans += canisters[i]
    return ans

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  