## CPP

### SOLUTION

long long maxScore(int n, vector<long long>& a, vector<long long>& b) {
    long long maxi = 0;
    long long mini = 0;

    for(int i = 0; i < n; ++i) {
        long long val1 = maxi - a[i];
        long long val2 = mini - a[i];
        long long val3 = b[i] - mini;
        long long val4 = b[i] - maxi;

        maxi = max({val1, val2, val3, val4});
        mini = min({val1, val2, val3, val4});
    }
    return maxi;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static long maxScore(int n, long[] a, long[] b) {
    long maxi = 0;
    long mini = 0;

    for (int i = 0; i < n; i++) {
        long val1 = maxi - a[i];
        long val2 = mini - a[i];
        long val3 = b[i] - mini;
        long val4 = b[i] - maxi;

        maxi = Math.max(val1, Math.max(val2, Math.max(val3, val4)));
        mini = Math.min(val1, Math.min(val2, Math.min(val3, val4)));
    }
    return maxi;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

long long maxScore(int n, long long* a, long long* b) {
    long long maxi = 0;
    long long mini = 0;

    for(int i = 0; i < n; ++i) {
        long long val1 = maxi - a[i];
        long long val2 = mini - a[i];
        long long val3 = b[i] - mini;
        long long val4 = b[i] - maxi;

        long long current_max = val1;
        if (val2 > current_max) current_max = val2;
        if (val3 > current_max) current_max = val3;
        if (val4 > current_max) current_max = val4;

        long long current_min = val1;
        if (val2 < current_min) current_min = val2;
        if (val3 < current_min) current_min = val3;
        if (val4 < current_min) current_min = val4;

        maxi = current_max;
        mini = current_min;
    }
    return maxi;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function maxScore(n, a, b) {
    let maxi = 0n;
    let mini = 0n;

    for (let i = 0; i < n; i++) {
        const val1 = maxi - BigInt(a[i]);
        const val2 = mini - BigInt(a[i]);
        const val3 = BigInt(b[i]) - mini;
        const val4 = BigInt(b[i]) - maxi;

        maxi = val1;
        if (val2 > maxi) maxi = val2;
        if (val3 > maxi) maxi = val3;
        if (val4 > maxi) maxi = val4;

        mini = val1;
        if (val2 < mini) mini = val2;
        if (val3 < mini) mini = val3;
        if (val4 < mini) mini = val4;
    }
    return maxi.toString();
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def maxScore(n: int, a: list, b: list) -> int:
    maxi = 0
    mini = 0

    for i in range(n):
        val1 = maxi - a[i]
        val2 = mini - a[i]
        val3 = b[i] - mini
        val4 = b[i] - maxi

        maxi = max(val1, val2, val3, val4)
        mini = min(val1, val2, val3, val4)
    
    return maxi

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  