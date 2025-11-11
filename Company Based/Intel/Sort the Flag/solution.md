## CPP

### SOLUTION

void sortColors(vector<int>& nums) {
    int low = 0;
    int mid = 0;
    int high = nums.size() - 1;

    while (mid <= high) {
        if (nums[mid] == 0) {
            swap(nums[low], nums[mid]);
            low++;
            mid++;
        } else if (nums[mid] == 1) {
            mid++;
        } else {
            swap(nums[mid], nums[high]);
            high--;
        }
    }
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static void sortColors(int[] nums) {
    int low = 0, mid = 0, high = nums.length - 1;

    while (mid <= high) {
        if (nums[mid] == 0) {
            int temp = nums[low];
            nums[low] = nums[mid];
            nums[mid] = temp;
            low++;
            mid++;
        } else if (nums[mid] == 1) {
            mid++;
        } else {
            int temp = nums[mid];
            nums[mid] = nums[high];
            nums[high] = temp;
            high--;
        }
    }
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

void sortColors(int* nums, int numsSize) {
    int low = 0, mid = 0, high = numsSize - 1;

    while (mid <= high) {
        if (nums[mid] == 0) {
            int temp = nums[low];
            nums[low] = nums[mid];
            nums[mid] = temp;
            low++;
            mid++;
        } else if (nums[mid] == 1) {
            mid++;
        } else {
            int temp = nums[mid];
            nums[mid] = nums[high];
            nums[high] = temp;
            high--;
        }
    }
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function sortColors(nums) {
    let low = 0, mid = 0, high = nums.length - 1;

    while (mid <= high) {
        if (nums[mid] === 0) {
            [nums[low], nums[mid]] = [nums[mid], nums[low]];
            low++;
            mid++;
        } else if (nums[mid] === 1) {
            mid++;
        } else {
            [nums[mid], nums[high]] = [nums[high], nums[mid]];
            high--;
        }
    }
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def sortColors(nums):
    low, mid, high = 0, 0, len(nums) - 1

    while mid <= high:
        if nums[mid] == 0:
            nums[low], nums[mid] = nums[mid], nums[low]
            low += 1
            mid += 1
        elif nums[mid] == 1:
            mid += 1
        else:
            nums[mid], nums[high] = nums[high], nums[mid]
            high -= 1

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  