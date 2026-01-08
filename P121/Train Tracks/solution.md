## CPP

### SOLUTION

long long minOperations(const std::vector<int>& arr) {
    std::map<int, int> counts;
    for (int x : arr) {
        counts[x]++;
    }
    
    long long operations = 0;
    for (auto const& [val, count] : counts) {
        operations += std::abs(count - 2);
    }
    return operations;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static long minOperations(int[] arr) {
    Map<Integer, Integer> counts = new HashMap<>();
    for (int x : arr) {
        counts.put(x, counts.getOrDefault(x, 0) + 1);
    }
    
    long operations = 0;
    for (int count : counts.values()) {
        operations += Math.abs(count - 2);
    }
    return operations;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

struct Entry {
    int key;
    int count;
};

int compareEntries(const void* a, const void* b) {
    const int* valA = (const int*)a;
    const int* valB = (const int*)b;
    if (*valA < *valB) return -1;
    if (*valA > *valB) return 1;
    return 0;
}

long long minOperations(int* arr, int n) {
    if (n == 0) return 0;
    
    // Sort to count frequencies easily
    qsort(arr, n, sizeof(int), compareEntries);
    
    long long operations = 0;
    int currentVal = arr[0];
    int currentCount = 1;
    
    for (int i = 1; i < n; i++) {
        if (arr[i] == currentVal) {
            currentCount++;
        } else {
            operations += abs(currentCount - 2);
            currentVal = arr[i];
            currentCount = 1;
        }
    }
    // Handle the last group
    operations += abs(currentCount - 2);
    
    return operations;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function minOperations(arr) {
    const counts = new Map();
    for (const x of arr) {
        counts.set(x, (counts.get(x) || 0) + 1);
    }
    
    let operations = 0;
    for (const count of counts.values()) {
        operations += Math.abs(count - 2);
    }
    return operations;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def minOperations(arr: list) -> int:
    counts = {}
    for x in arr:
        counts[x] = counts.get(x, 0) + 1
    
    operations = 0
    for count in counts.values():
        operations += abs(count - 2)
        
    return operations

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  