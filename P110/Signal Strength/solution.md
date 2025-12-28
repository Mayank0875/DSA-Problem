## CPP

### SOLUTION

int maxAscendingSum(vector<int>& nums) {
    if (nums.empty()) {
        return 0;
    }

    int maxSum = nums[0];
    int currentSum = nums[0];

    for (int i = 1; i < nums.size(); ++i) {
        if (nums[i] > nums[i - 1]) {
            currentSum += nums[i];
        } else {
            currentSum = nums[i];
        }
        maxSum = max(maxSum, currentSum);
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

public static int maxAscendingSum(int[] nums) {
    if (nums.length == 0) {
        return 0;
    }

    int maxSum = nums[0];
    int currentSum = nums[0];

    for (int i = 1; i < nums.length; i++) {
        if (nums[i] > nums[i - 1]) {
            currentSum += nums[i];
        } else {
            currentSum = nums[i];
        }
        maxSum = Math.max(maxSum, currentSum);
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

int maxAscendingSum(int* nums, int numsSize) {
    if (numsSize == 0) {
        return 0;
    }

    int maxSum = nums[0];
    int currentSum = nums[0];

    for (int i = 1; i < numsSize; i++) {
        if (nums[i] > nums[i - 1]) {
            currentSum += nums[i];
        } else {
            currentSum = nums[i];
        }
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

function maxAscendingSum(nums) {
    if (nums.length === 0) {
        return 0;
    }

    let maxSum = nums[0];
    let currentSum = nums[0];

    for (let i = 1; i < nums.length; i++) {
        if (nums[i] > nums[i - 1]) {
            currentSum += nums[i];
        } else {
            currentSum = nums[i];
        }
        maxSum = Math.max(maxSum, currentSum);
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

def maxAscendingSum(nums):
    if not nums:
        return 0

    max_sum = nums[0]
    current_sum = nums[0]

    for i in range(1, len(nums)):
        if nums[i] > nums[i - 1]:
            current_sum += nums[i]
        else:
            current_sum = nums[i]
        max_sum = max(max_sum, current_sum)

    return max_sum

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  