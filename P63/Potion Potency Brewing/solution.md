## CPP

### SOLUTION


int countVowelChants(int n) {    
    long long result = (long long)(n + 4) * (n + 3) * (n + 2) * (n + 1) / 24;
    return (int)result;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static int countVowelChants(int n) {
    long result = (long) (n + 4) * (n + 3) * (n + 2) * (n + 1) / 24;
    return (int) result;
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

int countVowelChants(int n) {
    long long result = (long long)(n + 4) * (n + 3) * (n + 2) * (n + 1) / 24;
    return (int)result;
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function countVowelChants(n) {
    const result = ((n + 4) * (n + 3) * (n + 2) * (n + 1)) / 24;
    return Math.floor(result);
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def countVowelChants(n):
    result = (n + 4) * (n + 3) * (n + 2) * (n + 1) // 24
    return result


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  