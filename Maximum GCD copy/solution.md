## CPP

### SOLUTION

bool findGrimoire(vector<int>& ids, int target) {
    int left = 0, right = ids.size() - 1;
    while (left <= right) {
        int mid = left + (right - left) / 2;

        if (ids[mid] == target) {
            return true;
        } else if (ids[mid] < target) {
            left = mid + 1;
        } else {
            right = mid - 1;
        }
    }
    return false;
}


### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## JAVA

### SOLUTION

public class Main {
    public static boolean findGrimoire(int[] ids, int target) {
        int left = 0, right = ids.length - 1;
        while (left <= right) {
            int mid = left + (right - left) / 2;
            if (ids[mid] == target) {
                return true;
            } else if (ids[mid] < target) {
                left = mid + 1;
            } else {
                right = mid - 1;
            }
        }
        return false;
    }
}


### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## C

### SOLUTION

bool findGrimoire(int arr[], int n, int target) {
    int left = 0, right = n - 1;
    while (left <= right) {
        int mid = left + (right - left) / 2;
        if (arr[mid] == target) {
            return true;
        } else if (arr[mid] < target) {
            left = mid + 1;
        } else {
            right = mid - 1;
        }
    }
    return false;
}

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## JAVASCRIPT

### SOLUTION

function findGrimoire(ids, target) {
    let left = 0, right = ids.length - 1;
    while (left <= right) {
        let mid = Math.floor(left + (right - left) / 2);
        if (ids[mid] === target) {
            return true;
        } else if (ids[mid] < target) {
            left = mid + 1;
        } else {
            right = mid - 1;
        }
    }
    return false;
}


### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## PYTHON

### SOLUTION

from typing import List

def findGrimoire(ids: List[int], target: int) -> bool:
    left, right = 0, len(ids) - 1
    while left <= right:
        mid = left + (right - left) // 2
        if ids[mid] == target:
            return True
        elif ids[mid] < target:
            left = mid + 1
        else:
            right = mid - 1
    return False

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256
