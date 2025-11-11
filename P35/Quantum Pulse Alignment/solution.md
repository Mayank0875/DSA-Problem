## CPP

### SOLUTION

bool check(long long s, long long w, long long h, long long n) {
    if (s < w || s < h) {
        return false;
    }
    long long cols = s / w;
    long long rows = s / h;
    if (cols == 0) return false; 
    long long required_rows = (n + cols - 1) / cols;
    return rows >= required_rows;
}

long long findMinSquareSide(long long w, long long h, long long n) {
    long long low = 1;
    long long high = 2e18; 
    long long ans = high;

    while (low <= high) {
        long long mid = low + (high - low) / 2;
        if (check(mid, w, h, n)) {
            ans = mid;
            high = mid - 1;
        } else {
            low = mid + 1; 
        }
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

public static boolean check(long s, long w, long h, long n) {
    if (s < w || s < h) {
        return false;
    }
    long cols = s / w;
    long rows = s / h;
    if (cols == 0) return false;
    long required_rows = (n + cols - 1) / cols;
    return rows >= required_rows;
}

public static long findMinSquareSide(long w, long h, long n) {
    long low = 1;
    long high = (long)2e18;
    long ans = high;

    while (low <= high) {
        long mid = low + (high - low) / 2;
        if (check(mid, w, h, n)) {
            ans = mid;
            high = mid - 1;
        } else {
            low = mid + 1;
        }
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

bool check(long long s, long long w, long long h, long long n) {
    if (s < w || s < h) {
        return false;
    }
    long long cols = s / w;
    long long rows = s / h;
    if (cols == 0) return false;
    long long required_rows = (n + cols - 1) / cols;
    return rows >= required_rows;
}

long long findMinSquareSide(long long w, long long h, long long n) {
    long long low = 1;
    long long high = 2000000000000000000LL;
    long long ans = high;

    while (low <= high) {
        long long mid = low + (high - low) / 2;
        if (check(mid, w, h, n)) {
            ans = mid;
            high = mid - 1;
        } else {
            low = mid + 1;
        }
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

function check(s, w, h, n) {
    if (s < w || s < h) return false;
    let cols = s / w;
    let rows = s / h;
    if (cols === 0) return false;
    let required_rows = Math.floor((n + cols - 1) / cols);
    return rows >= required_rows;
}

function findMinSquareSide(w, h, n) {
    let low = 1n;
    let high = 2000000000000000000n;
    let ans = high;

    while (low <= high) {
        let mid = low + (high - low) / 2n;
        if (check(Number(mid), Number(w), Number(h), Number(n))) {
            ans = mid;
            high = mid - 1n;
        } else {
            low = mid + 1n;
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

def check(s, w, h, n):
    if s < w or s < h:
        return False
    cols = s // w
    rows = s // h
    if cols == 0:
        return False
    required_rows = (n + cols - 1) // cols
    return rows >= required_rows

def findMinSquareSide(w, h, n):
    low, high = 1, 2 * 10**18
    ans = high

    while low <= high:
        mid = (low + high) // 2
        if check(mid, w, h, n):
            ans = mid
            high = mid - 1
        else:
            low = mid + 1
    return ans
    
### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  