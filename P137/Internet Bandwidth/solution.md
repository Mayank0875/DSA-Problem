## CPP

### SOLUTION

long long minOperations(vector<int>& a, vector<int>& b) {
    long long ops = 0;
    int n = a.size();
    for (int i = 0; i < n; ++i) {
        if (a[i] == b[i]) {
            continue;
        }
        // If one divides the other, we only need 1 operation (multiply the smaller one)
        if (a[i] % b[i] == 0 || b[i] % a[i] == 0) {
            ops += 1;
        } else {
            // Otherwise, we need 2 operations (multiply both to reach their LCM)
            ops += 2;
        }
    }
    return ops;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static long minOperations(int[] a, int[] b) {
    long ops = 0;
    int n = a.length;
    for (int i = 0; i < n; i++) {
        if (a[i] == b[i]) {
            continue;
        }
        // If one divides the other, we only need 1 operation
        if (a[i] % b[i] == 0 || b[i] % a[i] == 0) {
            ops += 1;
        } else {
            // Otherwise, we need 2 operations
            ops += 2;
        }
    }
    return ops;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

long long minOperations(int* a, int aSize, int* b, int bSize) {
    long long ops = 0;
    for (int i = 0; i < aSize; i++) {
        if (a[i] == b[i]) {
            continue;
        }
        if (a[i] % b[i] == 0 || b[i] % a[i] == 0) {
            ops += 1;
        } else {
            ops += 2;
        }
    }
    return ops;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function minOperations(a, b) {
    let ops = 0;
    const n = a.length;
    for (let i = 0; i < n; i++) {
        if (a[i] === b[i]) {
            continue;
        }
        if (a[i] % b[i] === 0 || b[i] % a[i] === 0) {
            ops += 1;
        } else {
            ops += 2;
        }
    }
    return ops;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def minOperations(a: list, b: list) -> int:
    ops = 0
    for x, y in zip(a, b):
        if x == y:
            continue
        if x % y == 0 or y % x == 0:
            ops += 1
        else:
            ops += 2
    return ops

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  