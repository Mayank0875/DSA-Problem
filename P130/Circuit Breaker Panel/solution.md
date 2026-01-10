## CPP

### SOLUTION

int countAligned(vector<int>& flips) {
    int n = flips.size();
    vector<bool> on(n, false);
    int maxBlue = 0;
    int result = 0;
    
    for (int i = 0; i < n; i++) {
        on[flips[i] - 1] = true;
        
        while (maxBlue < n && on[maxBlue]) {
            maxBlue++;
        }
        
        if (maxBlue == i + 1) {
            result++;
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

public static int countAligned(int[] flips) {
    int n = flips.length;
    boolean[] on = new boolean[n];
    int maxBlue = 0;
    int result = 0;
    
    for (int i = 0; i < n; i++) {
        // Turn on the bulb (convert 1-based index to 0-based)
        on[flips[i] - 1] = true;
        
        // Extend the prefix of ON bulbs starting from index 0
        while (maxBlue < n && on[maxBlue]) {
            maxBlue++;
        }
        
        // If the length of the continuous prefix equals the number of bulbs turned on
        if (maxBlue == i + 1) {
            result++;
        }
    }
    return result;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

int countAligned(int* flips, int flipsSize) {
    // Allocate boolean array initialized to false (0)
    bool* on = (bool*)calloc(flipsSize, sizeof(bool));
    int maxBlue = 0;
    int result = 0;
    
    for (int i = 0; i < flipsSize; i++) {
        on[flips[i] - 1] = true;
        
        while (maxBlue < flipsSize && on[maxBlue]) {
            maxBlue++;
        }
        
        if (maxBlue == i + 1) {
            result++;
        }
    }
    
    free(on);
    return result;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function countAligned(flips) {
    const n = flips.length;
    let on = new Array(n).fill(false);
    let maxBlue = 0;
    let result = 0;
    
    for (let i = 0; i < n; i++) {
        on[flips[i] - 1] = true;
        
        while (maxBlue < n && on[maxBlue]) {
            maxBlue++;
        }
        
        if (maxBlue === i + 1) {
            result++;
        }
    }
    return result;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def countAligned(flips: list) -> int:
    n = len(flips)
    on = [False] * n
    max_blue = 0
    result = 0
    
    for i in range(n):
        on[flips[i] - 1] = True
        
        while max_blue < n and on[max_blue]:
            max_blue += 1
            
        if max_blue == i + 1:
            result += 1
            
    return result

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  