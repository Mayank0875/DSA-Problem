## CPP

### SOLUTION

int findSmallestGem(vector<int>& gems) {
    int low = 0, high = gems.size() - 1;

    if (gems[low] <= gems[high]) {
        return gems[low];
    }

    while (low < high) {
        int mid = low + (high - low) / 2;
        if (mid > 0 && gems[mid] < gems[mid - 1]) {
             return gems[mid];
        }
        if (gems[mid] >= gems[low]) {
            low = mid + 1;
        }
        else {
            high = mid;
        }
    }
    return gems[low];
}


### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## JAVA

### SOLUTION

public static int findSmallestGem(int[] gems) {
    int low = 0, high = gems.length - 1;

    if (gems[low] <= gems[high]) {
        return gems[low];
    }

    while (low < high) {
        int mid = low + (high - low) / 2;
        if (mid > 0 && gems[mid] < gems[mid - 1]) {
            return gems[mid];
        }
        if (gems[mid] >= gems[low]) {
            low = mid + 1;
        } else {
            high = mid;
        }
    }
    return gems[low];
}


### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## C

### SOLUTION

int findSmallestGem(int arr[], int n) {
    int low = 0, high = n - 1;

    if (arr[low] <= arr[high]) {
        return arr[low];
    }

    while (low < high) {
        int mid = low + (high - low) / 2;
        if (mid > 0 && arr[mid] < arr[mid - 1]) {
            return arr[mid];
        }
        if (arr[mid] >= arr[low]) {
            low = mid + 1;
        } else {
            high = mid;
        }
    }
    return arr[low];
}

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## JAVASCRIPT

### SOLUTION

function findSmallestGem(gems) {
    let low = 0, high = gems.length - 1;

    if (gems[low] <= gems[high]) {
        return gems[low];
    }

    while (low < high) {
        let mid = Math.floor(low + (high - low) / 2);
        if (mid > 0 && gems[mid] < gems[mid - 1]) {
            return gems[mid];
        }
        if (gems[mid] >= gems[low]) {
            low = mid + 1;
        } else {
            high = mid;
        }
    }
    return gems[low];
}

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## PYTHON

### SOLUTION


def findSmallestGem(gems: List[int]) -> int:
    low, high = 0, len(gems) - 1

    if gems[low] <= gems[high]:
        return gems[low]

    while low < high:
        mid = low + (high - low) // 2
        if mid > 0 and gems[mid] < gems[mid - 1]:
            return gems[mid]
        if gems[mid] >= gems[low]:
            low = mid + 1
        else:
            high = mid
    return gems[low]

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256
