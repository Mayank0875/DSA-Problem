## CPP

### SOLUTION

int findGrimoire(vector<int>& ids, int target) {
    int left = 0, right = ids.size() - 1;
    while (left <= right) {
        int mid = left + (right - left) / 2;

        if (ids[mid] == target) {
            return 1;
        } else if (ids[mid] < target) {
            left = mid + 1;
        } else {
            right = mid - 1;
        }
    }
    return 0;
}


### METADATA

**TimeLimit**
1000

**MemoryLimit**
256

## JAVA

### SOLUTION

public static int findGrimoire(int[] ids, int target) {
    int left = 0, right = ids.length - 1;
    while (left <= right) {
        int mid = left + (right - left) / 2;
        if (ids[mid] == target) {
            return 1;
        } else if (ids[mid] < target) {
            left = mid + 1;
        } else {
            right = mid - 1;
        }
    }
    return 0;
}



### METADATA

**TimeLimit**
1000

**MemoryLimit**
256

## C

### SOLUTION

int findGrimoire(const int* ids, int n, int target) {
    int left = 0, right = n - 1;
    while (left <= right) {
        int mid = left + (right - left) / 2;
        if (ids[mid] == target) {
            return 1;
        } else if (ids[mid] < target) {
            left = mid + 1;
        } else {
            right = mid - 1;
        }
    }
    return 0;
}

### METADATA

**TimeLimit**
1000

**MemoryLimit**
256

## JAVASCRIPT

### SOLUTION

function findGrimoire(ids, target) {
    let left = 0, right = ids.length - 1;
    while (left <= right) {
        let mid = Math.floor(left + (right - left) / 2);
        if (ids[mid] === target) {
            return 1;
        } else if (ids[mid] < target) {
            left = mid + 1;
        } else {
            right = mid - 1;
        }
    }
    return 0;
}


### METADATA

**TimeLimit**
1000

**MemoryLimit**
256

## PYTHON

### SOLUTION


def findGrimoire(ids: List[int], target: int) -> bool:
    left, right = 0, len(ids) - 1
    while left <= right:
        mid = left + (right - left) // 2
        if ids[mid] == target:
            return 1
        elif ids[mid] < target:
            left = mid + 1
        else:
            right = mid - 1
    return 0

### METADATA

**TimeLimit**
1000

**MemoryLimit**
256
