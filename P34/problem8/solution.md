## CPP

### SOLUTION

long long count_less_equal(long long val, int n) {
    long long count = 0;
    for (int i = 1; i <= n; ++i) {
        count += min((long long)n, val / i);
    }
    return count;
}

long long TableMultiplication(long long n) {
    long long k = (n * n + 1) / 2;
    long long low = 1, high = n * n;
    long long ans = 0;

    while (low <= high) {
        long long mid = low + (high - low) / 2;
        if (count_less_equal(mid, n) >= k) {
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

public static long countLessEqual(long val, int n) {
    long count = 0;
    for (int i = 1; i <= n; ++i) {
        count += Math.min(n, val / i);
    }
    return count;
}

public static long TableMultiplication(long n) {
    long k = (n * n + 1) / 2;
    long low = 1, high = n * n;
    long ans = 0;

    while (low <= high) {
        long mid = low + (high - low) / 2;
        if (countLessEqual(mid, (int)n) >= k) {
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

long long count_less_equal(long long val, int n) {
    long long count = 0;
    for (int i = 1; i <= n; ++i) {
        count += (val / i < n ? val / i : n);
    }
    return count;
}

long long TableMultiplication(long long n) {
    long long k = (n * n + 1) / 2;
    long long low = 1, high = n * n;
    long long ans = 0;

    while (low <= high) {
        long long mid = low + (high - low) / 2;
        if (count_less_equal(mid, n) >= k) {
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

function countLessEqual(val, n) {
    let count = 0n;
    for (let i = 1n; i <= n; ++i) {
        count += (val / i < n ? val / i : n);
    }
    return count;
}

function TableMultiplication(n) {
    n = BigInt(n);
    let k = (n * n + 1n) / 2n;
    let low = 1n, high = n * n;
    let ans = 0n;

    while (low <= high) {
        let mid = low + (high - low) / 2n;
        if (countLessEqual(mid, n) >= k) {
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

def count_less_equal(val, n):
    count = 0
    for i in range(1, n + 1):
        count += min(n, val // i)
    return count

def TableMultiplication(n):
    k = (n * n + 1) // 2
    low, high = 1, n * n
    ans = 0

    while low <= high:
        mid = (low + high) // 2
        if count_less_equal(mid, n) >= k:
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