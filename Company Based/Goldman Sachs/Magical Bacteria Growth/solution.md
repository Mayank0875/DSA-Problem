## CPP

### SOLUTION

int findFinalValue(vector<int>& nums, int original) {
    set<int> numSet(nums.begin(), nums.end());
    
    while (numSet.count(original)) {
        original *= 2;
    }
    
    return original;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static int findFinalValue(List<Integer> nums, int original) {
    Set<Integer> numSet = new HashSet<>(nums);

    while (numSet.contains(original)) {
        original *= 2;
    }

    return original;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION


int findFinalValue(int* nums, int numsSize, int original) {
    bool exists = true;

    while (exists) {
        exists = false;
        for (int i = 0; i < numsSize; i++) {
            if (nums[i] == original) {
                original *= 2;
                exists = true;
                break;
            }
        }
    }

    return original;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function findFinalValue(nums, original) {
    const numSet = new Set(nums);

    while (numSet.has(original)) {
        original *= 2;
    }

    return original;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def findFinalValue(nums, original):
    num_set = set(nums)

    while original in num_set:
        original *= 2

    return original

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  