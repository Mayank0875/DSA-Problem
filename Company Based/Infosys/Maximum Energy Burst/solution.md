## CPP

### SOLUTION

int maxProduct(vector<int>& nums) {
    int n = nums.size();
    int maxProd = INT_MIN;
    int pref = 1, suff = 1;

    for (int i = 0; i < n; i++) {
        pref *= nums[i];
        suff *= nums[n - i - 1];
        maxProd = max(maxProd, max(pref, suff));

        if (pref == 0) pref = 1;
        if (suff == 0) suff = 1;
    }
    return maxProd;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static int maxProduct(int[] nums) {
    int n = nums.length;
    int maxProd = Integer.MIN_VALUE;
    int pref = 1, suff = 1;

    for (int i = 0; i < n; i++) {
        pref *= nums[i];
        suff *= nums[n - i - 1];
        maxProd = Math.max(maxProd, Math.max(pref, suff));

        if (pref == 0) pref = 1;
        if (suff == 0) suff = 1;
    }

    return maxProd;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION


int maxProduct(int* nums, int n) {
    int maxProd = INT_MIN;
    int pref = 1, suff = 1;

    for (int i = 0; i < n; i++) {
        pref *= nums[i];
        suff *= nums[n - i - 1];
        if (pref > maxProd) maxProd = pref;
        if (suff > maxProd) maxProd = suff;

        if (pref == 0) pref = 1;
        if (suff == 0) suff = 1;
    }
    return maxProd;
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function maxProduct(nums) {
    let n = nums.length;
    let maxProd = Number.MIN_SAFE_INTEGER;
    let pref = 1, suff = 1;

    for (let i = 0; i < n; i++) {
        pref *= nums[i];
        suff *= nums[n - i - 1];
        maxProd = Math.max(maxProd, pref, suff);

        if (pref === 0) pref = 1;
        if (suff === 0) suff = 1;
    }

    return maxProd;
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def maxProduct(self, nums: List[int]) -> int:
    n = len(nums)
    max_prod = float('-inf')
    pref = suff = 1

    for i in range(n):
        pref *= nums[i]
        suff *= nums[n - i - 1]
        max_prod = max(max_prod, pref, suff)

        if pref == 0:
            pref = 1
        if suff == 0:
            suff = 1
    
    return max_prod

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  