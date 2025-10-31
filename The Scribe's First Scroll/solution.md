## CPP

### SOLUTION

int findFirstScroll(vector<int>& ids, int target) {
    int low = 0;
    int high = ids.size();
    int ans = -1; 

    while (low < high) {
        int mid = low + (high - low) / 2;

        if (ids[mid] < target) {
            low = mid + 1;
        } else {
            high = mid;
        }
    }
    if (low < (int)ids.size() && ids[low] == target) {
        ans = low;
    }

    return ans;
}


### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## JAVA

### SOLUTION

public static int findFirstScroll(int[] ids, int target) {
    int left = 0, right = ids.length;
    int ans = -1;

    while (left < right) {
        int mid = left + (right - left) / 2;
        if (ids[mid] < target) {
            left = mid + 1;
        } else {
            right = mid;
        }
    }

    if (left < ids.length && ids[left] == target) {
        ans = left;
    }

    return ans;
}


### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## C

### SOLUTION

int findFirstScroll(int ids[], int n, int target) {
    int left = 0, right = n;
    int ans = -1;

    while (left < right) {
        int mid = left + (right - left) / 2;
        if (ids[mid] < target) {
            left = mid + 1;
        } else {
            right = mid;
        }
    }

    if (left < n && ids[left] == target) {
        ans = left;
    }

    return ans;
}

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## JAVASCRIPT

### SOLUTION

function findFirstScroll(ids, target) {
    let left = 0, right = ids.length;
    let ans = -1;

    while (left < right) {
        let mid = Math.floor(left + (right - left) / 2);
        if (ids[mid] < target) {
            left = mid + 1;
        } else {
            right = mid;
        }
    }

    if (left < ids.length && ids[left] === target) {
        ans = left;
    }

    return ans;
}


### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## PYTHON

### SOLUTION

def findFirstScroll(ids: List[int], target: int) -> int:
    left, right = 0, len(ids)
    ans = -1

    while left < right:
        mid = left + (right - left) // 2
        if ids[mid] < target:
            left = mid + 1
        else:
            right = mid

    if left < len(ids) and ids[left] == target:
        ans = left

    return ans

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256
