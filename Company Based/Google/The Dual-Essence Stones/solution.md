## CPP

### SOLUTION

int countPQPrimes(int n) {
    vector<int> prime_counts(n + 1, 0);

    for (int i = 2; i <= n; i++) {
        if (prime_counts[i] == 0) {
            for (int j = i; j <= n; j += i) {
                prime_counts[j]++;
            }
        }
    }

    int count = 0;
    for (int i = 1; i <= n; i++) {
        if (prime_counts[i] == 2) {
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

public static int countPQPrimes(int n) {
    int[] primeCounts = new int[n + 1];

    for (int i = 2; i <= n; i++) {
        if (primeCounts[i] == 0) {
            for (int j = i; j <= n; j += i) {
                primeCounts[j]++;
            }
        }
    }

    int count = 0;
    for (int i = 1; i <= n; i++) {
        if (primeCounts[i] == 2) {
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

int countPQPrimes(int n) {
    int* primeCounts = (int*)calloc(n + 1, sizeof(int));
    
    for (int i = 2; i <= n; i++) {
        if (primeCounts[i] == 0) {
            for (int j = i; j <= n; j += i) {
                primeCounts[j]++;
            }
        }
    }
    
    int count = 0;
    for (int i = 1; i <= n; i++) {
        if (primeCounts[i] == 2) {
            count++;
        }
    }
    
    free(primeCounts);
    return count;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function countPQPrimes(n) {
    const primeCounts = new Int32Array(n + 1).fill(0);

    for (let i = 2; i <= n; i++) {
        if (primeCounts[i] === 0) {
            for (let j = i; j <= n; j += i) {
                primeCounts[j]++;
            }
        }
    }

    let count = 0;
    for (let i = 1; i <= n; i++) {
        if (primeCounts[i] === 2) {
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

def countPQPrimes(n: int) -> int:
    prime_counts = [0] * (n + 1)
    
    for i in range(2, n + 1):
        if prime_counts[i] == 0:
            for j in range(i, n + 1, i):
                prime_counts[j] += 1
                
    count = 0
    for i in range(1, n + 1):
        if prime_counts[i] == 2:
            count += 1
            
    return count

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  