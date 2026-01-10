## CPP

### SOLUTION

int longestOnes(vector<int>& nums, int k) {
    int left = 0, right = 0;
    int zeroCount = 0;
    int maxLen = 0;
    int n = nums.size();

    for (right = 0; right < n; right++) {
        if (nums[right] == 0) {
            zeroCount++;
        }
        while (zeroCount > k) {
            if (nums[left] == 0) {
                zeroCount--;
            }
            left++;
        }
        maxLen = max(maxLen, (right - left + 1) - zeroCount);
    }
    return maxLen;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static int longestOnes(int[] nums, int k) {
    int left = 0;
    int zeroCount = 0;
    int maxLen = 0;
    
    for (int right = 0; right < nums.length; right++) {
        if (nums[right] == 0) {
            zeroCount++;
        }
        while (zeroCount > k) {
            if (nums[left] == 0) {
                zeroCount--;
            }
            left++;
        }
        maxLen = Math.max(maxLen, (right - left + 1) - zeroCount);
    }
    return maxLen;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

int longestOnes(int nums[], int n, int k) {
    int left = 0;
    int zeroCount = 0;
    int maxLen = 0;
    
    for (int right = 0; right < n; right++) {
        if (nums[right] == 0) {
            zeroCount++;
        }
        while (zeroCount > k) {
            if (nums[left] == 0) {
                zeroCount--;
            }
            left++;
        }
        int currentOnes = (right - left + 1) - zeroCount;
        if (currentOnes > maxLen) {
            maxLen = currentOnes;
        }
    }
    return maxLen;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function longestOnes(nums, k) {
    let left = 0;
    let zeroCount = 0;
    let maxLen = 0;
    
    for (let right = 0; right < nums.length; right++) {
        if (nums[right] === 0) {
            zeroCount++;
        }
        while (zeroCount > k) {
            if (nums[left] === 0) {
                zeroCount--;
            }
            left++;
        }
        maxLen = Math.max(maxLen, (right - left + 1) - zeroCount);
    }
    return maxLen;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def longestOnes(nums: list, k: int) -> int:
    left = 0
    zero_count = 0
    max_len = 0
    
    for right in range(len(nums)):
        if nums[right] == 0:
            zero_count += 1
            
        while zero_count > k:
            if nums[left] == 0:
                zero_count -= 1
            left += 1
            
        max_len = max(max_len, (right - left + 1) - zero_count)
        
    return max_len

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  