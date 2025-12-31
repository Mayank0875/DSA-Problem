## CPP

### SOLUTION

vector<int> getAverages(vector<int>& nums, int k) {
    int n = nums.size();
    long long windowSize = 2LL * k + 1;
    
    long long windowSum = 0;
    vector<int> result(n, -1);

    if (n < windowSize) {
        return result;
    }

    for (int i = 0; i < n; ++i) {
        windowSum += nums[i]; 

        if (i - windowSize >= 0) {
            windowSum -= nums[i - windowSize]; 
        }

        if (i >= windowSize - 1) {
            result[i - k] = windowSum / windowSize; 
        }
    }

    return result;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public int[] getAverages(int[] nums, int k) {
    int n = nums.length;
    long windowSize = 2L * k + 1;
    
    long windowSum = 0;
    int[] result = new int[n];
    Arrays.fill(result, -1);

    if (n < windowSize) {
        return result;
    }

    for (int i = 0; i < n; ++i) {
        windowSum += nums[i];

        if (i - windowSize >= 0) {
            windowSum -= nums[i - (int)windowSize];
        }

        if (i >= windowSize - 1) {
            result[i - k] = (int) (windowSum / windowSize);
        }
    }

    return result;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

int* getAverages(int* nums, int numsSize, int k, int* returnSize) {
    *returnSize = numsSize;
    int* result = (int*)malloc(numsSize * sizeof(int));
    for (int i = 0; i < numsSize; i++) {
        result[i] = -1;
    }
    
    long long windowSize = 2LL * k + 1;
    if (numsSize < windowSize) {
        return result;
    }
    
    long long windowSum = 0;
    for (int i = 0; i < numsSize; i++) {
        windowSum += nums[i];
        
        if (i >= windowSize) {
            windowSum -= nums[i - windowSize];
        }
        
        if (i >= windowSize - 1) {
            result[i - k] = (int)(windowSum / windowSize);
        }
    }
    return result;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

var getAverages = function(nums, k) {
    const n = nums.length;
    const windowSize = 2 * k + 1;
    const result = new Array(n).fill(-1);
    
    if (n < windowSize) return result;
    
    let windowSum = 0;
    for (let i = 0; i < n; i++) {
        windowSum += nums[i];
        
        if (i >= windowSize) {
            windowSum -= nums[i - windowSize];
        }
        
        if (i >= windowSize - 1) {
            result[i - k] = Math.floor(windowSum / windowSize);
        }
    }
    return result;
};

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def getAverages(self, nums: List[int], k: int) -> List[int]:
    n = len(nums)
    windowSize = 2 * k + 1

    windowSum = 0
    result = [-1] * n

    if n < windowSize:
        return result

    for i in range(n):
        windowSum += nums[i]

        if i - windowSize >= 0:
            windowSum -= nums[i - windowSize]

        if i >= windowSize - 1:
            result[i - k] = windowSum // windowSize

    return result

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  