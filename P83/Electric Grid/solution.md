## CPP

### SOLUTION

struct custom_hash {
    static uint64_t splitmix64(uint64_t x) {
        x += 0x9e3779b97f4a7c15;
        x = (x ^ (x >> 30)) * 0xbf58476d1ce4e5b9;
        x = (x ^ (x >> 27)) * 0x94d049bb133111eb;
        return x ^ (x >> 31);
    }

    size_t operator()(uint64_t x) const {
        static const uint64_t FIXED_RANDOM = chrono::steady_clock::now().time_since_epoch().count();
        return splitmix64(x + FIXED_RANDOM);
    }
};

long long countSubsetsWithSum(int n, int x, const vector<int>& t) {
    int n1 = n / 2;
    int n2 = n - n1;
    
    unordered_map<long long, int, custom_hash> sums_left;
    
    for (int i = 0; i < (1 << n1); ++i) {
        long long current_sum = 0;
        for (int j = 0; j < n1; ++j) {
            if ((i >> j) & 1) {
                current_sum += t[j];
            }
        }
        sums_left[current_sum]++;
    }
    
    long long count = 0;
    
    for (int i = 0; i < (1 << n2); ++i) {
        long long current_sum = 0;
        for (int j = 0; j < n2; ++j) {
            if ((i >> j) & 1) {
                current_sum += t[n1 + j];
            }
        }
        
        long long needed = x - current_sum;
        if (sums_left.count(needed)) {
            count += sums_left[needed];
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


public static long countSubsetsWithSum(int n, int x, int[] t) {
    int n1 = n / 2;
    int n2 = n - n1;
    
    Map<Long, Integer> sumsLeft = new HashMap<>();
    
    for (int i = 0; i < (1 << n1); i++) {
        long currentSum = 0;
        for (int j = 0; j < n1; j++) {
            if (((i >> j) & 1) == 1) {
                currentSum += t[j];
            }
        }
        sumsLeft.put(currentSum, sumsLeft.getOrDefault(currentSum, 0) + 1);
    }
    
    long count = 0;
    
    for (int i = 0; i < (1 << n2); i++) {
        long currentSum = 0;
        for (int j = 0; j < n2; j++) {
            if (((i >> j) & 1) == 1) {
                currentSum += t[n1 + j];
            }
        }
        
        long needed = x - currentSum;
        if (sumsLeft.containsKey(needed)) {
            count += sumsLeft.get(needed);
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

long long findMinimumBulbs(long long k) {
    long long left = 0;
    long long right = k + sqrtl(k) + 100;

    while (right - left > 1) {
        long long mid = (left + right) / 2;
        long long bulbsOn = mid - (long long)sqrtl(mid);

        if (bulbsOn < k)
            left = mid;
        else
            right = mid;
    }

    return right;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function findMinimumBulbs(k) {
    let left = 0n;
    let right = BigInt(k) + BigInt(Math.floor(Math.sqrt(Number(k)))) + 100n;

    while (right - left > 1n) {
        let mid = (left + right) / 2n;
        let bulbsOn = mid - BigInt(Math.floor(Math.sqrt(Number(mid))));

        if (bulbsOn < BigInt(k))
            left = mid;
        else
            right = mid;
    }

    return right;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def findMinimumBulbs(k):
    left = 0
    right = k + int(math.sqrt(k)) + 100

    while right - left > 1:
        mid = (left + right) // 2
        bulbs_on = mid - int(math.sqrt(mid))

        if bulbs_on < k:
            left = mid
        else:
            right = mid

    return right

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  