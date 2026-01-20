## CPP

### SOLUTION

vector<int> buildArray(vector<int>& nums) {
    int n = nums.size();

    for (int i = 0; i < n; ++i) {
        nums[i] += 1000 * (nums[nums[i]] % 1000);
    }
    for (int i = 0; i < n; ++i) {
        nums[i] /= 1000;
    }
    return nums;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public int[] buildArray(int[] nums) {
    int n = nums.length;
    // Encode both the old value and the new value into the array
    for (int i = 0; i < n; ++i) {
        nums[i] += 1000 * (nums[nums[i]] % 1000);
    }
    // Decode to get the new value
    for (int i = 0; i < n; ++i) {
        nums[i] /= 1000;
    }
    return nums;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

int* buildArray(int* nums, int numsSize, int* returnSize) {
    *returnSize = numsSize;
    // Store new value in higher digits
    for (int i = 0; i < numsSize; ++i) {
        nums[i] += 1000 * (nums[nums[i]] % 1000);
    }
    // Extract new value
    for (int i = 0; i < numsSize; ++i) {
        nums[i] /= 1000;
    }
    return nums;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

var buildArray = function(nums) {
    const n = nums.length;
    for (let i = 0; i < n; ++i) {
        nums[i] += 1000 * (nums[nums[i]] % 1000);
    }
    for (let i = 0; i < n; ++i) {
        nums[i] = Math.floor(nums[i] / 1000);
    }
    return nums;
};

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def buildArray(nums: list[int]) -> list[int]:
    n = len(nums)
    # Python handles large integers automatically, so no overflow issues
    for i in range(n):
        nums[i] += 1000 * (nums[nums[i]] % 1000)
    
    for i in range(n):
        nums[i] //= 1000
        
    return nums

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  