## CPP

### SOLUTION

int maxSubArray(vector<int>& nums) {
    int csum = nums[0];
    int tsum = nums[0];

    for (int i = 1; i < nums.size(); i++) {
        csum = max(nums[i], csum + nums[i]);
        tsum = max(tsum, csum);
    }
    return tsum;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static int maxSubArray(int[] nums) {
    int csum = nums[0];
    int tsum = nums[0];

    for (int i = 1; i < nums.length; i++) {
        csum = Math.max(nums[i], csum + nums[i]);
        tsum = Math.max(tsum, csum);
    }
    return tsum;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

int maxSubArray(int* nums, int n) {
    int csum = nums[0];
    int tsum = nums[0];

    for (int i = 1; i < n; i++) {
        if (csum + nums[i] > nums[i])
            csum = csum + nums[i];
        else
            csum = nums[i];

        if (tsum < csum)
            tsum = csum;
    }
    return tsum;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function maxSubArray(nums) {
    let csum = nums[0];
    let tsum = nums[0];

    for (let i = 1; i < nums.length; i++) {
        csum = Math.max(nums[i], csum + nums[i]);
        tsum = Math.max(tsum, csum);
    }

    return tsum;
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def maxSubArray(self, nums: List[int]) -> int:
    i=0
    csum=nums[0]
    tsum=nums[0]
    for i in range(1,len(nums)):
        csum= max(nums[i],csum+nums[i])
        tsum= max(tsum,csum)
    return tsum

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  