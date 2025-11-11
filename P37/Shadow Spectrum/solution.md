## CPP

### SOLUTION


bool check(long long t, long long n, long long x, long long y) {
    if (t < min(x, y)) {
        return false; 
    }

    long long time_after_first = t - min(x, y);
    long long copies_made = 1LL;
    if (x > 0) copies_made += time_after_first / x;
    if (y > 0) copies_made += time_after_first / y;

    return copies_made >= n;
}

long long MinimumTime(long long n, long long x, long long y) {
    long long low = 0; 
    long long high = n * max(x, y);
    long long ans = high; 

    while (low <= high) {
        long long mid = low + (high - low) / 2;
        if (check(mid, n, x, y)) {
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

public static boolean check(long t, long n, long x, long y) {
    if (t < Math.min(x, y)) {
        return false;
    }

    long timeAfterFirst = t - Math.min(x, y);
    long copiesMade = 1;
    copiesMade += timeAfterFirst / x;
    copiesMade += timeAfterFirst / y;

    return copiesMade >= n;
}

public static long MinimumTime(long n, long x, long y) {
    long low = 0, high = n * Math.max(x, y);
    long ans = high;

    while (low <= high) {
        long mid = low + (high - low) / 2;
        if (check(mid, n, x, y)) {
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

int check(long long t, long long n, long long x, long long y) {
    if (t < (x < y ? x : y)) {
        return 0; // false
    }

    long long time_after_first = t - (x < y ? x : y);
    long long copies_made = 1;
    copies_made += time_after_first / x;
    copies_made += time_after_first / y;

    return copies_made >= n;
}

long long MinimumTime(long long n, long long x, long long y) {
    long long low = 0;
    long long high = n * (x > y ? x : y);
    long long ans = high;

    while (low <= high) {
        long long mid = low + (high - low) / 2;
        if (check(mid, n, x, y)) {
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

function check(t, n, x, y) {
    if (t < Math.min(x, y)) return false;

    let timeAfterFirst = t - Math.min(x, y);
    let copiesMade = 1;
    copiesMade += Math.floor(timeAfterFirst / x);
    copiesMade += Math.floor(timeAfterFirst / y);

    return copiesMade >= n;
}

function MinimumTime(n, x, y) {
    let low = 0n;
    let high = BigInt(n) * BigInt(Math.max(x, y));
    let ans = high;

    while (low <= high) {
        let mid = (low + high) / 2n;
        if (check(Number(mid), n, x, y)) {
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

def check(t, n, x, y):
    if t < min(x, y):
        return False
    
    time_after_first = t - min(x, y)
    copies_made = 1
    copies_made += time_after_first // x
    copies_made += time_after_first // y
    
    return copies_made >= n

def MinimumTime(n, x, y):
    low, high = 0, n * max(x, y)
    ans = high

    while low <= high:
        mid = (low + high) // 2
        if check(mid, n, x, y):
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