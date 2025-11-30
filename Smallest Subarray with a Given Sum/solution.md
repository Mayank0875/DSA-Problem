## CPP

### SOLUTION
int minSubArrayLen(int target, vector<int>& nums) {
    int n = nums.size();
    if (n == 0) {
        return 0;
    }
    int ans = INT_MAX;
    int left = 0;
    int sum = 0;
    for (int i = 0; i < n; i++) {
        sum += nums[i];
        while (sum >= target) {
            ans = min(ans, i + 1 - left);
            sum -= nums[left++];
        }
    }
    return (ans != INT_MAX) ? ans : 0;
}


### METADATA

**TimeLimit**
1000

**MemoryLimit**
256

## JAVA

### SOLUTION

public static int minSubArrayLen(int target, int[] nums) {
    int n = nums.length;
    if (n == 0) {
        return 0;
    }
    int ans = Integer.MAX_VALUE;
    int left = 0;
    int sum = 0;
    for (int i = 0; i < n; i++) {
        sum += nums[i];
        while (sum >= target) {
            ans = Math.min(ans, i + 1 - left);
            sum -= nums[left++];
        }
    }
    return (ans != Integer.MAX_VALUE) ? ans : 0;
}


### METADATA

**TimeLimit**
1000

**MemoryLimit**
256

## C

### SOLUTION

int minSubArrayLen(int target, int* nums, int n) {
    if (n == 0)
        return 0;

    int ans = INT_MAX;
    int left = 0;
    int sum = 0;

    for (int i = 0; i < n; i++) {
        sum += nums[i];
        while (sum >= target) {
            int len = i + 1 - left;
            if (len < ans)
                ans = len;
            sum -= nums[left++];
        }
    }

    return (ans != INT_MAX) ? ans : 0;
}

### METADATA

**TimeLimit**
1000

**MemoryLimit**
256

## JAVASCRIPT

### SOLUTION

function minSubArrayLen(target, nums) {
    const n = nums.length;
    if (n === 0) return 0;

    let ans = Number.MAX_SAFE_INTEGER;
    let left = 0, sum = 0;

    for (let i = 0; i < n; i++) {
        sum += nums[i];
        while (sum >= target) {
            ans = Math.min(ans, i + 1 - left);
            sum -= nums[left++];
        }
    }

    return ans !== Number.MAX_SAFE_INTEGER ? ans : 0;
}


### METADATA

**TimeLimit**
1000

**MemoryLimit**
256

## PYTHON

### SOLUTION



def minSubArrayLen(target, nums):
    n = len(nums)
    if n == 0:
        return 0

    ans = float('inf')
    left = 0
    total = 0

    for i in range(n):
        total += nums[i]
        while total >= target:
            ans = min(ans, i + 1 - left)
            total -= nums[left]
            left += 1

    return ans if ans != float('inf') else 0

### METADATA

**TimeLimit**
1000

**MemoryLimit**
256
