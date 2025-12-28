## CPP

### SOLUTION

int solveTimeline(vector<int>& arr) {
    int right = arr.size() - 1;
    while (right > 0 && arr[right] >= arr[right - 1]) {
        right--;
    }

    int ans = right;
    int left = 0;
    while (left < right && (left == 0 || arr[left - 1] <= arr[left])) {
        // find next valid number after arr[left]
        while (right < arr.size() && arr[left] > arr[right]) {
            right++;
        }
        // save length of removed subarray
        ans = min(ans, right - left - 1);
        left++;
    }
    return ans;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static int solveTimeline(int[] arr) {
    int right = arr.length - 1;
    while (right > 0 && arr[right] >= arr[right - 1]) {
        right--;
    }

    int ans = right;
    int left = 0;
    while (left < right && (left == 0 || arr[left - 1] <= arr[left])) {
        // find next valid number after arr[left]
        while (right < arr.length && arr[left] > arr[right]) {
            right++;
        }
        // save length of removed subarray
        ans = Math.min(ans, right - left - 1);
        left++;
    }
    return ans;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

int solveTimeline(int* arr, int n) {
    int right = n - 1;
    while (right > 0 && arr[right] >= arr[right - 1]) {
        right--;
    }

    int ans = right;
    int left = 0;
    while (left < right && (left == 0 || arr[left - 1] <= arr[left])) {
        // find next valid number after arr[left]
        while (right < n && arr[left] > arr[right]) {
            right++;
        }
        // save length of removed subarray
        int removed = right - left - 1;
        if (removed < ans) {
            ans = removed;
        }
        left++;
    }
    return ans;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function solveTimeline(arr) {
    let right = arr.length - 1;
    while (right > 0 && arr[right] >= arr[right - 1]) {
        right--;
    }

    let ans = right;
    let left = 0;
    while (left < right && (left === 0 || arr[left - 1] <= arr[left])) {
        // find next valid number after arr[left]
        while (right < arr.length && arr[left] > arr[right]) {
            right++;
        }
        // save length of removed subarray
        ans = Math.min(ans, right - left - 1);
        left++;
    }
    return ans;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def solveTimeline(arr: list) -> int:
    right = len(arr) - 1
    while right > 0 and arr[right] >= arr[right - 1]:
        right -= 1

    ans = right
    left = 0
    while left < right and (left == 0 or arr[left - 1] <= arr[left]):
        # find next valid number after arr[left]
        while right < len(arr) and arr[left] > arr[right]:
            right += 1
        # save length of removed subarray
        ans = min(ans, right - left - 1)
        left += 1
    return ans

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  