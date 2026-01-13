## CPP

### SOLUTION

int minCostToLightUp(int n, string s) {
    s += s;
    int max_zeros = 0;
    int current_zeros = 0;
    
    for (char c : s) {
        if (c == '1') {
            current_zeros = 0;
        } else {
            current_zeros++;
            max_zeros = max(max_zeros, current_zeros);
        }
    }
    return max_zeros;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static int minCostToLightUp(int n, String s) {
    String doubled = s + s;
    int maxZeros = 0;
    int currentZeros = 0;
    
    for (int i = 0; i < doubled.length(); i++) {
        if (doubled.charAt(i) == '1') {
            currentZeros = 0;
        } else {
            currentZeros++;
            maxZeros = Math.max(maxZeros, currentZeros);
        }
    }
    return maxZeros;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

int minCostToLightUp(int n, char* s) {
    int max_zeros = 0;
    int current_zeros = 0;
    
    // We simulate iterating over s + s
    for (int i = 0; i < 2 * n; i++) {
        char c = s[i % n];
        if (c == '1') {
            current_zeros = 0;
        } else {
            current_zeros++;
            if (current_zeros > max_zeros) {
                max_zeros = current_zeros;
            }
        }
    }
    return max_zeros;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function minCostToLightUp(n, s) {
    let doubled = s + s;
    let maxZeros = 0;
    let currentZeros = 0;
    
    for (let char of doubled) {
        if (char === '1') {
            currentZeros = 0;
        } else {
            currentZeros++;
            maxZeros = Math.max(maxZeros, currentZeros);
        }
    }
    return maxZeros;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def minCostToLightUp(n: int, s: str) -> int:
    doubled = s + s
    groups = doubled.split('1')
    if not groups:
        return 0
    return max(len(g) for g in groups)

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  