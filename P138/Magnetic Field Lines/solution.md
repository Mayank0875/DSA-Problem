## CPP

### SOLUTION

long long countCompatible(long long x, long long m) {
    long long count = 0;
    long long limit = m;
    if (2 * x < limit) {
        limit = 2 * x;
    }

    for (long long y = 1; y <= limit; ++y) {
        long long val = x ^ y;
        if (val == 0) continue; // x cannot equal y
        
        if (x % val == 0 || y % val == 0) {
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


## JAVA

### SOLUTION

public static long countCompatible(long x, long m) {
    long count = 0;
    long limit = (m < 2 * x) ? m : 2 * x;

    for (long y = 1; y <= limit; y++) {
        long val = x ^ y;
        if (val == 0) continue;

        if (x % val == 0 || y % val == 0) {
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



## C

### SOLUTION

long long countCompatible(long long x, long long m) {
    long long count = 0;
    long long limit = m;
    if (2 * x < limit) {
        limit = 2 * x;
    }

    for (long long y = 1; y <= limit; ++y) {
        long long val = x ^ y;
        if (val == 0) continue;

        if (x % val == 0 || y % val == 0) {
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

function countCompatible(x, m) {
    let count = 0;
    let limit = BigInt(m);
    let limitNum;
    
    if (BigInt(2 * x) < limit) {
        limitNum = 2 * x;
    } else {
        limitNum = Number(m); 
    }

    for (let y = 1; y <= limitNum; y++) {
        let val = x ^ y;
        if (val === 0) continue;

        if (x % val === 0 || y % val === 0) {
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



## PYTHON

### SOLUTION

def countCompatible(x: int, m: int) -> int:
    count = 0
    limit = min(m, 2 * x)
    
    for y in range(1, limit + 1):
        val = x ^ y
        if val == 0:
            continue
            
        if x % val == 0 or y % val == 0:
            count += 1
            
    return count

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  