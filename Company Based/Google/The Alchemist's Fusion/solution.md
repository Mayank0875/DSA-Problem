## CPP

### SOLUTION

long long countPerfectPairs(int n, int k, vector<int>& a) {
    const int MAX_VAL = 100005;
    vector<int> spf(MAX_VAL);
    for (int i = 0; i < MAX_VAL; ++i) spf[i] = i;
    for (int i = 2; i * i < MAX_VAL; ++i) {
        if (spf[i] == i) {
            for (int j = i * i; j < MAX_VAL; j += i)
                if (spf[j] == j) spf[j] = i;
        }
    }

    vector<int> freq(MAX_VAL, 0);
    long long ans = 0;

    for (int x : a) {
        long long normalized = 1;
        long long required = 1;
        int temp = x;
        
        while (temp > 1) {
            int p = spf[temp];
            int count = 0;
            while (temp % p == 0) {
                count++;
                temp /= p;
            }
            
            int rem = count % k;
            if (rem > 0) {
                for (int i = 0; i < rem; ++i) normalized *= p;
                
                int need = k - rem;
                for (int i = 0; i < need; ++i) {
                    required *= p;
                    if (required >= MAX_VAL) break;
                }
            }
        }

        if (required < MAX_VAL) {
            ans += freq[required];
        }
        freq[normalized]++;
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

public static long countPerfectPairs(int n, int k, int[] a) {
    int MAX_VAL = 100005;
    int[] spf = new int[MAX_VAL];
    for (int i = 0; i < MAX_VAL; i++) spf[i] = i;
    for (int i = 2; i * i < MAX_VAL; i++) {
        if (spf[i] == i) {
            for (int j = i * i; j < MAX_VAL; j += i)
                if (spf[j] == j) spf[j] = i;
        }
    }

    int[] freq = new int[MAX_VAL];
    long ans = 0;

    for (int x : a) {
        long normalized = 1;
        long required = 1;
        int temp = x;

        while (temp > 1) {
            int p = spf[temp];
            int count = 0;
            while (temp % p == 0) {
                count++;
                temp /= p;
            }

            int rem = count % k;
            if (rem > 0) {
                for (int i = 0; i < rem; i++) normalized *= p;

                int need = k - rem;
                for (int i = 0; i < need; i++) {
                    required *= p;
                    if (required >= MAX_VAL) break;
                }
            }
        }

        if (required < MAX_VAL) {
            ans += freq[(int)required];
        }
        if (normalized < MAX_VAL) {
            freq[(int)normalized]++;
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

#define MAX_VAL 100005

int spf[MAX_VAL];
int freq[MAX_VAL];

void precompute() {
    for (int i = 0; i < MAX_VAL; ++i) spf[i] = i;
    for (int i = 2; i * i < MAX_VAL; ++i) {
        if (spf[i] == i) {
            for (int j = i * i; j < MAX_VAL; j += i)
                if (spf[j] == j) spf[j] = i;
        }
    }
}

long long countPerfectPairs(int n, int k, int* a) {
    if (spf[2] == 0) precompute(); 
    
    // Clear freq array for each test case if reused
    for(int i=0; i<MAX_VAL; i++) freq[i] = 0;

    long long ans = 0;

    for (int i = 0; i < n; i++) {
        long long normalized = 1;
        long long required = 1;
        int temp = a[i];
        
        while (temp > 1) {
            int p = spf[temp];
            int count = 0;
            while (temp % p == 0) {
                count++;
                temp /= p;
            }
            
            int rem = count % k;
            if (rem > 0) {
                for (int l = 0; l < rem; ++l) normalized *= p;
                
                int need = k - rem;
                for (int l = 0; l < need; ++l) {
                    required *= p;
                    if (required >= MAX_VAL) break;
                }
            }
        }

        if (required < MAX_VAL) {
            ans += freq[required];
        }
        if (normalized < MAX_VAL) {
            freq[normalized]++;
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

function countPerfectPairs(n, k, a) {
    const MAX_VAL = 100005;
    const spf = new Int32Array(MAX_VAL);
    for (let i = 0; i < MAX_VAL; i++) spf[i] = i;
    for (let i = 2; i * i < MAX_VAL; i++) {
        if (spf[i] === i) {
            for (let j = i * i; j < MAX_VAL; j += i)
                if (spf[j] === j) spf[j] = i;
        }
    }

    const freq = new Int32Array(MAX_VAL);
    let ans = 0n;

    for (let x of a) {
        let normalized = 1;
        let required = 1;
        let temp = x;
        
        while (temp > 1) {
            let p = spf[temp];
            let count = 0;
            while (temp % p === 0) {
                count++;
                temp = Math.floor(temp / p);
            }
            
            let rem = count % k;
            if (rem > 0) {
                for (let i = 0; i < rem; ++i) normalized *= p;
                
                let need = k - rem;
                for (let i = 0; i < need; ++i) {
                    required *= p;
                    if (required >= MAX_VAL) break;
                }
            }
        }

        if (required < MAX_VAL) {
            ans += BigInt(freq[required]);
        }
        if (normalized < MAX_VAL) {
            freq[normalized]++;
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

def countPerfectPairs(n, k, a):
    MAX_VAL = 100005
    spf = list(range(MAX_VAL))
    for i in range(2, int(MAX_VAL**0.5) + 1):
        if spf[i] == i:
            for j in range(i*i, MAX_VAL, i):
                if spf[j] == j:
                    spf[j] = i
    
    freq = [0] * MAX_VAL
    ans = 0
    
    for x in a:
        normalized = 1
        required = 1
        temp = x
        
        while temp > 1:
            p = spf[temp]
            count = 0
            while temp % p == 0:
                count += 1
                temp //= p
            
            rem = count % k
            if rem > 0:
                normalized *= (p ** rem)
                
                need = k - rem
                # Check for overflow relative to MAX_VAL to avoid huge numbers
                for _ in range(need):
                    required *= p
                    if required >= MAX_VAL:
                        break
        
        if required < MAX_VAL:
            ans += freq[required]
        
        if normalized < MAX_VAL:
            freq[normalized] += 1
            
    return ans

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  