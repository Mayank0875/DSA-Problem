## CPP

### SOLUTION

int findInsertPosition(vector<int>& ids, int target) {
    int left = 0, right = ids.size(); 
    while (left < right) {
        int mid = left + (right - left) / 2;
        if (ids[mid] < target) {
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

## JAVA

### SOLUTION

public class Main {
    public static int findInsertPosition(int[] ids, int target) {
        int left = 0, right = ids.length;
        while (left < right) {
            int mid = left + (right - left) / 2;
            if (ids[mid] < target) {
                left = mid + 1;
            } else {
                right = mid;
            }
        }
        return left;
    }
}


### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## C

### SOLUTION

int findInsertPosition(int arr[], int n, int target) {
    int left = 0, right = n;
    while (left < right) {
        int mid = left + (right - left) / 2;
        if (arr[mid] < target) {
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

function findInsertPosition(ids, target) {
    let left = 0, right = ids.length;
    while (left < right) {
        let mid = Math.floor(left + (right - left) / 2);
        if (ids[mid] < target) {
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


def findInsertPosition(ids: List[int], target: int) -> int:
    left, right = 0, len(ids)
    while left < right:
        mid = left + (right - left) // 2
        if ids[mid] < target:
            left = mid + 1
        else:
            right = mid
    return left

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256
