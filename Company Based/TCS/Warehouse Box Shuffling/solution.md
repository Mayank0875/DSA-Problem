## CPP

### SOLUTION

vector<int> moveZeroesToEnd(vector<int>& nums) {
    int insertPos = 0;
    for (int i = 0; i < nums.size(); ++i) {
        if (nums[i] != 0) {
            std::swap(nums[insertPos], nums[i]);
            insertPos++;
        }
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

public static List<Integer> moveZeroesToEnd(List<Integer> nums) {
    int insertPos = 0;
    for (int i = 0; i < nums.size(); i++) {
        if (nums.get(i) != 0) {
            Collections.swap(nums, insertPos, i);
            insertPos++;
        }
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


int* moveZeroesToEnd(int* nums, int size) {
    int insertPos = 0;
    for (int i = 0; i < size; i++) {
        if (nums[i] != 0) {
            int temp = nums[insertPos];
            nums[insertPos] = nums[i];
            nums[i] = temp;
            insertPos++;
        }
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

function moveZeroesToEnd(nums) {
    let insertPos = 0;
    for (let i = 0; i < nums.length; i++) {
        if (nums[i] !== 0) {
            [nums[insertPos], nums[i]] = [nums[i], nums[insertPos]];
            insertPos++;
        }
    }

    return nums;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def moveZeroesToEnd(nums):
    insert_pos = 0
    for i in range(len(nums)):
        if nums[i] != 0:
            nums[insert_pos], nums[i] = nums[i], nums[insert_pos]
            insert_pos += 1

    return nums

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  