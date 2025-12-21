## CPP

### SOLUTION

long long minCost(int n, int k) {
    if (n == 2) {
        if ((k & (k - 1))) {
            return 0;
        } else {
            return 1;
        }
    }

    if (n % 2 != 0) {
        long long sum = (long long)(n / 2) * 3;
        if (sum < k) {
            return 0;
        }
        sum++;
        long long ex = k - sum;
        return std::abs(ex * 2);
    } else {
        long long f = (n - 1) / 2;
        long long c = n / 2;
        long long sum1 = f * 2 + c;
        long long rem = k - sum1;
        
        if ((rem - 2) < 0) {
            return (std::abs(rem - 2) - 1) * 2 + 1;
        }
        if ((rem & 1) == 0) {
            return 0;
        }
        if ((rem - 1) == 2) {
            return 1;
        }
        return 0;
    }
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static long minCost(int n, int k) {
    if (n == 2) {
        if ((k & (k - 1)) != 0) {
            return 0;
        } else {
            return 1;
        }
    }

    if (n % 2 != 0) {
        long sum = (long)(n / 2) * 3;
        if (sum < k) {
            return 0;
        }
        sum++;
        long ex = k - sum;
        return Math.abs(ex * 2);
    } else {
        long f = (n - 1) / 2;
        long c = n / 2;
        long sum1 = f * 2 + c;
        long rem = k - sum1;

        if ((rem - 2) < 0) {
            return (Math.abs(rem - 2) - 1) * 2 + 1;
        }
        if ((rem & 1) == 0) {
            return 0;
        }
        if ((rem - 1) == 2) {
            return 1;
        }
        return 0;
    }
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  
