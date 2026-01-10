## CPP

### SOLUTION

bool check(long long r, int n, int m, const vector<long long>& cities, const vector<long long>& towers) {
    int i = 0; // index for cities
    int j = 0; // index for towers
    while (i < n && j < m) {
        long long leftBound = towers[j] - r;
        long long rightBound = towers[j] + r;
        if (cities[i] >= leftBound && cities[i] <= rightBound) {
            // City i is covered by tower j
            i++;
        } else {
            // Try next tower
            j++;
        }
    }
    return i == n;
}

long long minRadius(int n, int m, vector<long long>& cities, vector<long long>& towers) {
    long long left = 0, right = 2000000000000000000LL; // 2e18
    long long ans = right;

    while (left <= right) {
        long long mid = left + (right - left) / 2;
        if (check(mid, n, m, cities, towers)) {
            ans = mid;
            right = mid - 1;
        } else {
            left = mid + 1;
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

public static boolean check(long r, int n, int m, long[] cities, long[] towers) {
    int i = 0; 
    int j = 0; 
    while (i < n && j < m) {
        long leftBound = towers[j] - r;
        long rightBound = towers[j] + r;
        if (cities[i] >= leftBound && cities[i] <= rightBound) {
            i++;
        } else {
            j++;
        }
    }
    return i == n;
}

public static long minRadius(int n, int m, long[] cities, long[] towers) {
    long left = 0;
    long right = 2000000000000000000L;
    long ans = right;

    while (left <= right) {
        long mid = left + (right - left) / 2;
        if (check(mid, n, m, cities, towers)) {
            ans = mid;
            right = mid - 1;
        } else {
            left = mid + 1;
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

int check(long long r, int n, int m, long long* cities, long long* towers) {
    int i = 0;
    int j = 0;
    while (i < n && j < m) {
        long long leftBound = towers[j] - r;
        long long rightBound = towers[j] + r;
        if (cities[i] >= leftBound && cities[i] <= rightBound) {
            i++;
        } else {
            j++;
        }
    }
    return i == n;
}

long long minRadius(int n, int m, long long* cities, long long* towers) {
    long long left = 0;
    long long right = 2000000000000000000LL;
    long long ans = right;

    while (left <= right) {
        long long mid = left + (right - left) / 2;
        if (check(mid, n, m, cities, towers)) {
            ans = mid;
            right = mid - 1;
        } else {
            left = mid + 1;
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

function check(r, n, m, cities, towers) {
    let i = 0;
    let j = 0;
    while (i < n && j < m) {
        // Use BigInt logic
        let leftBound = towers[j] - r;
        let rightBound = towers[j] + r;
        if (cities[i] >= leftBound && cities[i] <= rightBound) {
            i++;
        } else {
            j++;
        }
    }
    return i === n;
}

function minRadius(n, m, cities, towers) {
    let left = 0n;
    let right = 2000000000000000000n;
    let ans = right;

    // Convert inputs to BigInt for safe comparison
    const bigCities = cities.map(BigInt);
    const bigTowers = towers.map(BigInt);

    while (left <= right) {
        let mid = (left + right) / 2n;
        if (check(mid, n, m, bigCities, bigTowers)) {
            ans = mid;
            right = mid - 1n;
        } else {
            left = mid + 1n;
        }
    }
    return ans.toString();
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def check(r: int, n: int, m: int, cities: list, towers: list) -> bool:
    i = 0
    j = 0
    while i < n and j < m:
        leftBound = towers[j] - r
        rightBound = towers[j] + r
        if leftBound <= cities[i] <= rightBound:
            i += 1
        else:
            j += 1
    return i == n

def minRadius(n: int, m: int, cities: list, towers: list) -> int:
    left = 0
    right = 2 * 10**18
    ans = right
    
    while left <= right:
        mid = (left + right) // 2
        if check(mid, n, m, cities, towers):
            ans = mid
            right = mid - 1
        else:
            left = mid + 1
            
    return ans

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  