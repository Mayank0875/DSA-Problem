## CPP

### SOLUTION

bool canSqrt(long long x, long long mid) {
    return mid * mid <= x;
}

long long integerSquareRoot(long long x) {
    long long l = 0, h = x, ans = 0;
    while (l <= h) {
        long long mid = (l + h) / 2;
        if (canSqrt(x, mid)) { ans = mid; l = mid + 1; }
        else h = mid - 1;
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

public static boolean canSqrt(long x, long mid) {
    return mid * mid <= x;
}

public static long integerSquareRoot(long x) {
    long l = 0, h = x, ans = 0;
    while (l <= h) {
        long mid = (l + h) / 2;
        if (canSqrt(x, mid)) { ans = mid; l = mid + 1; }
        else h = mid - 1;
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


bool canSqrt(long long x, long long mid) {
    return mid * mid <= x;
}

long long integerSquareRoot(long long x) {
    long long l = 0, h = x, ans = 0;
    while (l <= h) {
        long long mid = (l + h) / 2;
        if (canSqrt(x, mid)) { ans = mid; l = mid + 1; }
        else h = mid - 1;
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

function canSqrt(x, mid) {
    return mid * mid <= x;
}

function integerSquareRoot(x) {
    x = BigInt(x);  
    let l = 0n, h = x, ans = 0n;
    while (l <= h) {
        let mid = (l + h) >> 1n;  
        if (canSqrt(x, mid)) {
            ans = mid;
            l = mid + 1n;
        } else {
            h = mid - 1n;
        }
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

def integerSquareRoot(x: int) -> int:
    l, h, ans = 0, x, 0
    while l <= h:
        mid = (l + h) // 2
        if mid * mid <= x:
            ans = mid
            l = mid + 1
        else:
            h = mid - 1
    return ans

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  