## CPP

### SOLUTION

bool duplicate(vector<int>& nums, int k) {
    unordered_set<int> window;
    int left = 0;
    for (int right = 0; right < nums.size(); right++) {
        if (window.count(nums[right])) return true;
        window.insert(nums[right]);
        if (right - left >= k) {
            window.erase(nums[left]);
            left++;
        }
    }
    return false;
}

### METADATA

**TimeLimit**
1000

**MemoryLimit** 
512

## JAVA

### SOLUTION

public static boolean duplicate(int[] nums, int k) {
    Set<Integer> window = new HashSet<>();
    int left = 0;
    for (int right = 0; right < nums.length; right++) {
        if (window.contains(nums[right])) return true;
        window.add(nums[right]);
        if (right - left >= k) {
            window.remove(nums[left]);
            left++;
        }
    }
    return false;
}

### METADATA

**TimeLimit**
1000

**MemoryLimit**
512

## C

### SOLUTION

bool duplicate(int n, int* nums, int k) {
    for (int i = 0; i < n; i++) {
        for (int j = i + 1; j <= i + k && j < n; j++) {
            if (nums[i] == nums[j]) return true;
        }
    }
    return false;
}


### METADATA

**TimeLimit**
1000

**MemoryLimit**
512

## JAVASCRIPT

### SOLUTION

function duplicate(nums, k) {
  const set = new Set();
  let left = 0;
  for (let right = 0; right < nums.length; right++) {
    if (set.has(nums[right])) return true;
    set.add(nums[right]);
    if (right - left >= k) {
      set.delete(nums[left]);
      left++;
    }
  }
  return false;
}

### METADATA

**TimeLimit**
1000

**MemoryLimit**
512

## PYTHON

### SOLUTION

def duplicate(nums, k):
    seen = set()
    left = 0
    for right in range(len(nums)):
        if nums[right] in seen:
            return True
        seen.add(nums[right])
        if right - left >= k:
            seen.remove(nums[left])
            left += 1
    return False

### METADATA

**TimeLimit**
1000

**MemoryLimit**
512