## CPP

### SOLUTION

vector<int> rotateArray(vector<int>& nums, int k) {
    int n = nums.size();
    if (n == 0) return nums;
    
    k = k % n; 
    if (k == 0) return nums;
    reverse(nums.begin(), nums.end());
    reverse(nums.begin(), nums.begin() + k);
    reverse(nums.begin() + k, nums.end());

    return nums;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static List<Integer> rotateArray(List<Integer> nums, int k) {
    int n = nums.size();
    if (n == 0) return nums;

    k = k % n;
    if (k == 0) return nums;

    Collections.reverse(nums);
    Collections.reverse(nums.subList(0, k));
    Collections.reverse(nums.subList(k, n));

    return nums;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

void reverse(int* nums, int start, int end) {
    while (start < end) {
        int temp = nums[start];
        nums[start] = nums[end];
        nums[end] = temp;
        start++;
        end--;
    }
}

int* rotateArray(int* nums, int n, int k) {
    if (n == 0) return nums;

    k = k % n;
    if (k == 0) return nums;

    reverse(nums, 0, n - 1);
    reverse(nums, 0, k - 1);
    reverse(nums, k, n - 1);

    return nums;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function rotateArray(nums, k) {
    const n = nums.length;
    if (n === 0) return nums;

    k = k % n;
    if (k === 0) return nums;

    nums.reverse();
    nums = [...nums.slice(0, k).reverse(), ...nums.slice(k).reverse()];

    return nums;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def rotateArray(nums, k):
    n = len(nums)
    if n == 0:
        return nums

    k = k % n
    if k == 0:
        return nums

    nums.reverse()
    nums[:k] = reversed(nums[:k])
    nums[k:] = reversed(nums[k:])

    return nums

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  