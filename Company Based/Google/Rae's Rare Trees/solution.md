## CPP

### SOLUTION

bool solve(int n, vector<int>& p) {
    vector<int> pre(n);
    vector<int> suf(n);
    
    pre[0] = p[0];
    for(int i = 1; i < n; i++) {
        pre[i] = min(pre[i-1], p[i]);
    }
    
    suf[n-1] = p[n-1];
    for(int i = n - 2; i >= 0; i--) {
        suf[i] = max(suf[i+1], p[i]);
    }
    
    // Check splits between i and i+1
    for(int i = 0; i < n - 1; i++) {
        if(pre[i] > suf[i+1]) {
            return false;
        }
    }
    
    return true;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public boolean solve(int n, int[] p) {
    int[] pre = new int[n];
    int[] suf = new int[n];
    
    pre[0] = p[0];
    for (int i = 1; i < n; i++) {
        pre[i] = Math.min(pre[i - 1], p[i]);
    }
    
    suf[n - 1] = p[n - 1];
    for (int i = n - 2; i >= 0; i--) {
        suf[i] = Math.max(suf[i + 1], p[i]);
    }
    
    for (int i = 0; i < n - 1; i++) {
        if (pre[i] > suf[i + 1]) {
            return false;
        }
    }
    
    return true;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

#define MIN(a,b) (((a)<(b))?(a):(b))
#define MAX(a,b) (((a)>(b))?(a):(b))

bool solve(int n, int* p) {
    int* pre = (int*)malloc(n * sizeof(int));
    int* suf = (int*)malloc(n * sizeof(int));
    
    pre[0] = p[0];
    for (int i = 1; i < n; i++) {
        pre[i] = MIN(pre[i - 1], p[i]);
    }
    
    suf[n - 1] = p[n - 1];
    for (int i = n - 2; i >= 0; i--) {
        suf[i] = MAX(suf[i + 1], p[i]);
    }
    
    bool possible = true;
    for (int i = 0; i < n - 1; i++) {
        if (pre[i] > suf[i + 1]) {
            possible = false;
            break;
        }
    }
    
    free(pre);
    free(suf);
    return possible;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

var solve = function(n, p) {
    const pre = new Int32Array(n);
    const suf = new Int32Array(n);
    
    pre[0] = p[0];
    for (let i = 1; i < n; i++) {
        pre[i] = Math.min(pre[i - 1], p[i]);
    }
    
    suf[n - 1] = p[n - 1];
    for (let i = n - 2; i >= 0; i--) {
        suf[i] = Math.max(suf[i + 1], p[i]);
    }
    
    for (let i = 0; i < n - 1; i++) {
        if (pre[i] > suf[i + 1]) {
            return false;
        }
    }
    
    return true;
};

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def solve(n: int, p: list) -> bool:
    pre = [0] * n
    suf = [0] * n
    
    pre[0] = p[0]
    for i in range(1, n):
        pre[i] = min(pre[i-1], p[i])
        
    suf[n-1] = p[n-1]
    for i in range(n-2, -1, -1):
        suf[i] = max(suf[i+1], p[i])
        
    for i in range(n - 1):
        if pre[i] > suf[i+1]:
            return False
            
    return True

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  