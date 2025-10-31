## CPP

### SOLUTION

long long countUpTo(long long n) {
    if (n < 1) {
        return 0;
    }
    long long low = 1, high = 2e9;
    long long ans = 0;
    while (low <= high) {
        long long mid = low + (high - low) / 2;
        if (mid > n / mid) { 
            high = mid - 1;
        } else {
            ans = mid;
            low = mid + 1;
        }
    }
    return ans;
}

long long countPerfectSquaresInRange(long long L, long long R) {
    return countUpTo(R) - countUpTo(L - 1);
}


### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## JAVA

### SOLUTION


public static long countUpTo(long n) {
    if (n < 1) {
        return 0;
    }
    long low = 1, high = 2000000000L;
    long ans = 0;

    while (low <= high) {
        long mid = low + (high - low) / 2;
        if (mid > n / mid) {
            high = mid - 1;
        } else {
            ans = mid;
            low = mid + 1;
        }
    }
    return ans;
}

public static long countPerfectSquaresInRange(long L, long R) {
    return countUpTo(R) - countUpTo(L - 1);
}



### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## C

### SOLUTION

long long countUpTo(long long n) {
    if (n < 1) {
        return 0;
    }
    long long low = 1, high = 2000000000LL;
    long long ans = 0;

    while (low <= high) {
        long long mid = low + (high - low) / 2;
        if (mid > n / mid) {
            high = mid - 1;
        } else {
            ans = mid;
            low = mid + 1;
        }
    }
    return ans;
}

long long countPerfectSquaresInRange(long long L, long long R) {
    return countUpTo(R) - countUpTo(L - 1);
}

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## JAVASCRIPT

### SOLUTION

function countUpTo(n) {
    n = BigInt(n);
    if (n < 1n) return 0n;

    let low = 1n, high = 2000000000n;
    let ans = 0n;

    while (low <= high) {
        let mid = (low + high) >> 1n; 
        if (mid > n / mid) {
            high = mid - 1n;
        } else {
            ans = mid;
            low = mid + 1n;
        }
    }

    return ans;
}

function countPerfectSquaresInRange(L, R) {
    L = BigInt(L);
    R = BigInt(R);
    return countUpTo(R) - countUpTo(L - 1n);
}

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## PYTHON

### SOLUTION

def countUpTo(n: int) -> int:
    if n < 1:
        return 0

    low, high = 1, 2000000000
    ans = 0

    while low <= high:
        mid = low + (high - low) // 2
        if mid > n // mid:
            high = mid - 1
        else:
            ans = mid
            low = mid + 1

    return ans


def countPerfectSquaresInRange(L: int, R: int) -> int:
    return countUpTo(R) - countUpTo(L - 1)

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256
