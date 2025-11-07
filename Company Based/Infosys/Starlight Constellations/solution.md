## CPP

### SOLUTION

long long countConstellations(vector<int>& nums, long long target) {
    int n = nums.size();
    if (n < 4) {
        return 0;
    }
    
    sort(nums.begin(), nums.end());
    long long count = 0;

    for (int i = 0; i < n - 3; ++i) {
        if (i > 0 && nums[i] == nums[i - 1]) {
            continue;
        }

        for (int j = i + 1; j < n - 2; ++j) {
            if (j > i + 1 && nums[j] == nums[j - 1]) {
                continue;
            }

            int left = j + 1;
            int right = n - 1;
            
            while (left < right) {
                long long current_sum = (long long)nums[i] + nums[j] + nums[left] + nums[right];
                
                if (current_sum == target) {
                    count++;
                    while (left < right && nums[left] == nums[left + 1]) {
                        left++;
                    }
                    while (left < right && nums[right] == nums[right - 1]) {
                        right--;
                    }
                    left++;
                    right--;
                } else if (current_sum < target) {
                    left++;
                } else {
                    right--;
                }
            }
        }
    }
    return count;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static long countConstellations(int[] nums, long target) {
    int n = nums.length;
    if (n < 4) {
        return 0;
    }

    Arrays.sort(nums);
    long count = 0;

    for (int i = 0; i < n - 3; i++) {
        if (i > 0 && nums[i] == nums[i - 1]) continue;

        for (int j = i + 1; j < n - 2; j++) {
            if (j > i + 1 && nums[j] == nums[j - 1]) continue;

            int left = j + 1;
            int right = n - 1;

            while (left < right) {
                long currentSum = (long) nums[i] + nums[j] + nums[left] + nums[right];

                if (currentSum == target) {
                    count++;
                    while (left < right && nums[left] == nums[left + 1]) left++;
                    while (left < right && nums[right] == nums[right - 1]) right--;
                    left++;
                    right--;
                } else if (currentSum < target) {
                    left++;
                } else {
                    right--;
                }
            }
        }
    }

    return count;
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

int compare(const void *a, const void *b) {
    return (*(int*)a - *(int*)b);
}

long long countConstellations(int* nums, int n, long long target) {
    if (n < 4) return 0;

    qsort(nums, n, sizeof(int), compare);
    long long count = 0;

    for (int i = 0; i < n - 3; i++) {
        if (i > 0 && nums[i] == nums[i - 1]) continue;

        for (int j = i + 1; j < n - 2; j++) {
            if (j > i + 1 && nums[j] == nums[j - 1]) continue;

            int left = j + 1;
            int right = n - 1;

            while (left < right) {
                long long current_sum = (long long)nums[i] + nums[j] + nums[left] + nums[right];

                if (current_sum == target) {
                    count++;
                    while (left < right && nums[left] == nums[left + 1]) left++;
                    while (left < right && nums[right] == nums[right - 1]) right--;
                    left++;
                    right--;
                } else if (current_sum < target) {
                    left++;
                } else {
                    right--;
                }
            }
        }
    }

    return count;
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function countConstellations(nums, target) {
    const n = nums.length;
    if (n < 4) return 0;

    nums.sort((a, b) => a - b);
    let count = 0n;
    target = BigInt(target);

    for (let i = 0; i < n - 3; i++) {
        if (i > 0 && nums[i] === nums[i - 1]) continue;

        for (let j = i + 1; j < n - 2; j++) {
            if (j > i + 1 && nums[j] === nums[j - 1]) continue;

            let left = j + 1;
            let right = n - 1;

            while (left < right) {
                let currentSum = BigInt(nums[i]) + BigInt(nums[j]) + BigInt(nums[left]) + BigInt(nums[right]);

                if (currentSum === target) {
                    count++;
                    while (left < right && nums[left] === nums[left + 1]) left++;
                    while (left < right && nums[right] === nums[right - 1]) right--;
                    left++;
                    right--;
                } else if (currentSum < target) {
                    left++;
                } else {
                    right--;
                }
            }
        }
    }

    return Number(count);
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def countConstellations(nums, target):
    n = len(nums)
    if n < 4:
        return 0

    nums.sort()
    count = 0

    for i in range(n - 3):
        if i > 0 and nums[i] == nums[i - 1]:
            continue

        for j in range(i + 1, n - 2):
            if j > i + 1 and nums[j] == nums[j - 1]:
                continue

            left = j + 1
            right = n - 1

            while left < right:
                current_sum = nums[i] + nums[j] + nums[left] + nums[right]

                if current_sum == target:
                    count += 1
                    while left < right and nums[left] == nums[left + 1]:
                        left += 1
                    while left < right and nums[right] == nums[right - 1]:
                        right -= 1
                    left += 1
                    right -= 1
                elif current_sum < target:
                    left += 1
                else:
                    right -= 1

    return count


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  