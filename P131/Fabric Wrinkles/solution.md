## CPP

### SOLUTION

int minSteps(int num) {
    if (num == 0) return 0;
    vector<int> dp(num + 1, 1e9);
    dp[0] = 0;
    
    for (int i = 1; i <= num; i++) {
        int temp = i;
        while (temp > 0) {
            int digit = temp % 10;
            temp /= 10;
            if (digit > 0) {
                dp[i] = min(dp[i], dp[i - digit] + 1);
            }
        }
    }
    return dp[num];
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static int minSteps(int num) {
    if (num == 0) return 0;
    int[] dp = new int[num + 1];
    Arrays.fill(dp, 1000000000);
    dp[0] = 0;
    
    for (int i = 1; i <= num; i++) {
        int temp = i;
        while (temp > 0) {
            int digit = temp % 10;
            temp /= 10;
            if (digit > 0) {
                dp[i] = Math.min(dp[i], dp[i - digit] + 1);
            }
        }
    }
    return dp[num];
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

int min(int a, int b) {
    return (a < b) ? a : b;
}

int minSteps(int num) {
    if (num == 0) return 0;
    int* dp = (int*)malloc((num + 1) * sizeof(int));
    
    dp[0] = 0;
    for(int i = 1; i <= num; i++) dp[i] = 1000000000;
    
    for (int i = 1; i <= num; i++) {
        int temp = i;
        while (temp > 0) {
            int digit = temp % 10;
            temp /= 10;
            if (digit > 0) {
                dp[i] = min(dp[i], dp[i - digit] + 1);
            }
        }
    }
    
    int result = dp[num];
    free(dp);
    return result;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function minSteps(num) {
    if (num === 0) return 0;
    let dp = new Int32Array(num + 1).fill(1000000000);
    dp[0] = 0;
    
    for (let i = 1; i <= num; i++) {
        let temp = i;
        while (temp > 0) {
            let digit = temp % 10;
            temp = Math.floor(temp / 10);
            if (digit > 0) {
                dp[i] = Math.min(dp[i], dp[i - digit] + 1);
            }
        }
    }
    return dp[num];
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def minSteps(num: int) -> int:
    if num == 0:
        return 0
    dp = [float('inf')] * (num + 1)
    dp[0] = 0
    
    for i in range(1, num + 1):
        temp = i
        while temp > 0:
            digit = temp % 10
            temp //= 10
            if digit > 0:
                dp[i] = min(dp[i], dp[i - digit] + 1)
                
    return dp[num]

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  