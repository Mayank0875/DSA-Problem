## CPP

### SOLUTION

long long solveResonance(int n, const std::vector<long long>& a) {
    if (n == 1) {
        return a[0];
    }
    
    long long sum = 0;
    for (long long x : a) {
        sum += x;
    }
    
    long long ans = sum;
    ans ^= (sum - a[0]);
    ans ^= (sum - a[n - 1]);
    ans ^= (sum - a[0] - a[n - 1]);
    
    return ans;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static long solveResonance(int n, long[] a) {
    if (n == 1) {
        return a[0];
    }
    
    long sum = 0;
    for (long x : a) {
        sum += x;
    }
    
    long ans = sum;
    ans ^= (sum - a[0]);
    ans ^= (sum - a[n - 1]);
    ans ^= (sum - a[0] - a[n - 1]);
    
    return ans;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  

