## CPP

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


## JAVA

### SOLUTION

public static long findMinimumBulbs(long k) {
    long left = 0;
    long right = k + (long)Math.sqrt(k) + 100;

    while (right - left > 1) {
        long mid = (left + right) / 2;
        long bulbsOn = mid - (long)Math.sqrt(mid);

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