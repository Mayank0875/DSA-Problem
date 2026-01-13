## CPP

### SOLUTION

long long maxDifference(int n, vector<long long>& a) {
    vector<long long> prefix(n + 1, 0);
    for (int i = 0; i < n; ++i) {
        prefix[i + 1] = prefix[i] + a[i];
    }

    long long maxDiff = 0;

    for (int k = 1; k <= n; ++k) {
        if (n % k == 0) {
            long long currentMin = -1;
            long long currentMax = -1;
            
            for (int i = 0; i < n; i += k) {
                long long truckWeight = prefix[i + k] - prefix[i];
                
                if (currentMin == -1 || truckWeight < currentMin) {
                    currentMin = truckWeight;
                }
                if (currentMax == -1 || truckWeight > currentMax) {
                    currentMax = truckWeight;
                }
            }
            
            if (currentMax - currentMin > maxDiff) {
                maxDiff = currentMax - currentMin;
            }
        }
    }
    return maxDiff;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static long maxDifference(int n, long[] a) {
    long[] prefix = new long[n + 1];
    prefix[0] = 0;
    for (int i = 0; i < n; i++) {
        prefix[i + 1] = prefix[i] + a[i];
    }

    long maxDiff = 0;

    for (int k = 1; k <= n; k++) {
        if (n % k == 0) {
            long currentMin = Long.MAX_VALUE;
            long currentMax = Long.MIN_VALUE;

            for (int i = 0; i < n; i += k) {
                long truckWeight = prefix[i + k] - prefix[i];
                if (truckWeight < currentMin) currentMin = truckWeight;
                if (truckWeight > currentMax) currentMax = truckWeight;
            }
            
            if (currentMin != Long.MAX_VALUE) {
                maxDiff = Math.max(maxDiff, currentMax - currentMin);
            }
        }
    }
    return maxDiff;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

long long maxDifference(int n, long long* a) {
    long long* prefix = (long long*)malloc((n + 1) * sizeof(long long));
    prefix[0] = 0;
    for (int i = 0; i < n; ++i) {
        prefix[i + 1] = prefix[i] + a[i];
    }

    long long maxDiff = 0;

    for (int k = 1; k <= n; ++k) {
        if (n % k == 0) {
            long long currentMin = -1;
            long long currentMax = -1;

            for (int i = 0; i < n; i += k) {
                long long truckWeight = prefix[i + k] - prefix[i];

                if (currentMin == -1 || truckWeight < currentMin) {
                    currentMin = truckWeight;
                }
                if (currentMax == -1 || truckWeight > currentMax) {
                    currentMax = truckWeight;
                }
            }
            
            if (currentMax - currentMin > maxDiff) {
                maxDiff = currentMax - currentMin;
            }
        }
    }
    free(prefix);
    return maxDiff;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function maxDifference(n, a) {
    // Use BigInt for potentially large sums
    const prefix = new BigInt64Array(n + 1);
    prefix[0] = 0n;
    for (let i = 0; i < n; i++) {
        prefix[i + 1] = prefix[i] + BigInt(a[i]);
    }

    let maxDiff = 0n;

    for (let k = 1; k <= n; k++) {
        if (n % k === 0) {
            let currentMin = -1n;
            let currentMax = -1n;

            for (let i = 0; i < n; i += k) {
                let truckWeight = prefix[i + k] - prefix[i];

                if (currentMin === -1n || truckWeight < currentMin) {
                    currentMin = truckWeight;
                }
                if (currentMax === -1n || truckWeight > currentMax) {
                    currentMax = truckWeight;
                }
            }

            let diff = currentMax - currentMin;
            if (diff > maxDiff) {
                maxDiff = diff;
            }
        }
    }
    return maxDiff.toString();
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def maxDifference(n: int, a: list) -> int:
    prefix = [0] * (n + 1)
    for i in range(n):
        prefix[i + 1] = prefix[i] + a[i]
        
    max_diff = 0
    
    # Iterate over all possible truck sizes k
    for k in range(1, n + 1):
        if n % k == 0:
            current_min = float('inf')
            current_max = float('-inf')
            
            # Check segments
            for i in range(0, n, k):
                truck_weight = prefix[i + k] - prefix[i]
                if truck_weight < current_min:
                    current_min = truck_weight
                if truck_weight > current_max:
                    current_max = truck_weight
            
            if current_max - current_min > max_diff:
                max_diff = current_max - current_min
                
    return max_diff

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  