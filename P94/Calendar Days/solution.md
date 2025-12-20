## CPP

### SOLUTION

int minSteps(int n) {
    int res = 0;
    while (n > 0) {
        int max_digit = 0;
        int temp = n;
        while (temp > 0) {
            int digit = temp % 10;
            if (digit > max_digit) {
                max_digit = digit;
            }
            temp /= 10;
        }
        n -= max_digit;
        res++;
    }
    return res;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static int minSteps(int n) {
    int res = 0;
    while (n > 0) {
        int maxDigit = 0;
        int temp = n;
        while (temp > 0) {
            int digit = temp % 10;
            if (digit > maxDigit) {
                maxDigit = digit;
            }
            temp /= 10;
        }
        n -= maxDigit;
        res++;
    }
    return res;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  

