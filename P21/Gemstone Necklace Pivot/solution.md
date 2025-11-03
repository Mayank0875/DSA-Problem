## CPP

### SOLUTION

int findSmallest(vector<int>& arr) {
    int low = 0, high = arr.size() - 1;

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
        }
        else {
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

## JAVA

### SOLUTION

public static int findSmallest(int[] arr) {
    int low = 0, high = arr.length - 1;

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

## C

### SOLUTION

int findSmallest(int arr[], int n) {
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

function findSmallest(arr) {
    let low = 0, high = arr.length - 1;

    if (arr[low] <= arr[high]) {
        return arr[low];
    }

    while (low < high) {
        let mid = Math.floor(low + (high - low) / 2);
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

## PYTHON

### SOLUTION


def findSmallest(arr: List[int]) -> int:
    low, high = 0, len(arr) - 1

    if arr[low] <= arr[high]:
        return arr[low]

    while low < high:
        mid = low + (high - low) // 2
        if mid > 0 and arr[mid] < arr[mid - 1]:
            return arr[mid]
        if arr[mid] >= arr[low]:
            low = mid + 1
        else:
            high = mid
    return arr[low]

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256
