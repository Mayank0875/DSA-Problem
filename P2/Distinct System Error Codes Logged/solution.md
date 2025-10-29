## CPP

### SOLUTION

int countDistinctArtifacts(vector<int>& codes) {
    set<int> distinct_codes(codes.begin(), codes.end());
    return distinct_codes.size();
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static int countDistinctArtifacts(int[] codes) {
    Set<Integer> distinctCodes = new HashSet<>();
    for (int code : codes) distinctCodes.add(code);
    return distinctCodes.size();
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

int countDistinctArtifacts(int* codes, int n) {
    qsort(codes, n, sizeof(int), compare);
    int count = (n > 0) ? 1 : 0;
    for (int i = 1; i < n; ++i) {
        if (codes[i] != codes[i - 1]) {
            count++;
        }
    }
    return count;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function countDistinctArtifacts(codes) {
    const distinctCodes = new Set(codes);
    return distinctCodes.size;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def countDistinctArtifacts(codes):
    return len(set(codes))

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  