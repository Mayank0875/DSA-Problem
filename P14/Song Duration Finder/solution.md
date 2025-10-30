## CPP

### SOLUTION

int findSectionEnd(const vector<int>& ids, int target) {
    int low = 0;
    int high = ids.size(); 

    while (low < high) {
        int mid = low + (high - low) / 2;

        if (ids[mid] <= target) {
            low = mid + 1;
        } else {
            high = mid;
        }
    }
    return low;
}


### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## JAVA

### SOLUTION

public static int findSectionEnd(int[] ids, int target) {
    int left = 0, right = ids.length;
    while (left < right) {
        int mid = left + (right - left) / 2;
        if (ids[mid] <= target) {
            left = mid + 1;
        } else {
            right = mid;
        }
    }
    return left;
}


### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## C

### SOLUTION

int findSectionEnd(const int* ids, int n, int target) {
    int left = 0, right = n;
    while (left < right) {
        int mid = left + (right - left) / 2;
        if (ids[mid] <= target) {
            left = mid + 1;
        } else {
            right = mid;
        }
    }
    return left;
}

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## JAVASCRIPT

### SOLUTION

function findSectionEnd(ids, target) {
    let left = 0, right = ids.length;
    while (left < right) {
        let mid = Math.floor(left + (right - left) / 2);
        if (ids[mid] <= target) {
            left = mid + 1;
        } else {
            right = mid;
        }
    }
    return left;
}


### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## PYTHON

### SOLUTION


def findSectionEnd(ids: List[int], target: int) -> int:
    left, right = 0, len(ids)
    while left < right:
        mid = left + (right - left) // 2
        if ids[mid] <= target:
            left = mid + 1
        else:
            right = mid
    return left

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256
