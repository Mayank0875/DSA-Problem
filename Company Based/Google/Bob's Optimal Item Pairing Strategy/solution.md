## CPP

### SOLUTION

int minPairSum(std::vector<int>& nums) {
    std::sort(nums.begin(), nums.end());
    int maxSum = 0;
    int n = nums.size();
    for (int i = 0; i < n / 2; i++) {
        int currentSum = nums[i] + nums[n - 1 - i];
        if (currentSum > maxSum) {
            maxSum = currentSum;
        }
    }
    return maxSum;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public int minPairSum(int[] nums) {
    Arrays.sort(nums);
    int maxSum = 0;
    int n = nums.length;
    for (int i = 0; i < n / 2; i++) {
        maxSum = Math.max(maxSum, nums[i] + nums[n - 1 - i]);
    }
    return maxSum;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

int compare(const void* a, const void* b) {
    return (*(int*)a - *(int*)b);
}

int minPairSum(int* nums, int numsSize) {
    qsort(nums, numsSize, sizeof(int), compare);
    int maxSum = 0;
    for (int i = 0; i < numsSize / 2; i++) {
        int currentSum = nums[i] + nums[numsSize - 1 - i];
        if (currentSum > maxSum) {
            maxSum = currentSum;
        }
    }
    return maxSum;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function minPairSum(nums) {
    nums.sort((a, b) => a - b);
    let maxSum = 0;
    let n = nums.length;
    for (let i = 0; i < n / 2; i++) {
        maxSum = Math.max(maxSum, nums[i] + nums[n - 1 - i]);
    }
    return maxSum;
}
### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def minPairSum(nums):
    nums.sort()
    max_sum = 0
    n = len(nums)
    for i in range(n // 2):
        max_sum = max(max_sum, nums[i] + nums[n - 1 - i])
    return max_sum

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  