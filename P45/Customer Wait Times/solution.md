## CPP

### SOLUTION

int firstOccurrence(vector<int>& arr, int target) {
    int low = 0, high = arr.size() - 1;
    int ans = -1;
    while (low <= high) {
        int mid = low + (high - low) / 2;
        if (arr[mid] == target) {
            ans = mid;
            high = mid - 1; 
        } else if (arr[mid] < target) {
            low = mid + 1;
        } else {
            high = mid - 1;
        }
    }
    return ans;
}

int lastOccurrence(vector<int>& arr, int target) {
    int low = 0, high = arr.size() - 1;
    int ans = -1;
    while (low <= high) {
        int mid = low + (high - low) / 2;
        if (arr[mid] == target) {
            ans = mid;
            low = mid + 1; 
        } else if (arr[mid] < target) {
            low = mid + 1;
        } else {
            high = mid - 1;
        }
    }
    return ans;
}

int countOccurrences(vector<int>& arr, int target) {
    int first = firstOccurrence(arr, target);
    if (first == -1) return 0;
    int last = lastOccurrence(arr, target);
    return last - first + 1;
}

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## JAVA

### SOLUTION


public static int firstOccurrence(int[] arr, int target) {
    int low = 0, high = arr.length - 1;
    int ans = -1;
    while (low <= high) {
        int mid = low + (high - low) / 2;
        if (arr[mid] == target) {
            ans = mid;
            high = mid - 1;
        } else if (arr[mid] < target) {
            low = mid + 1;
        } else {
            high = mid - 1;
        }
    }
    return ans;
}

public static int lastOccurrence(int[] arr, int target) {
    int low = 0, high = arr.length - 1;
    int ans = -1;
    while (low <= high) {
        int mid = low + (high - low) / 2;
        if (arr[mid] == target) {
            ans = mid;
            low = mid + 1;
        } else if (arr[mid] < target) {
            low = mid + 1;
        } else {
            high = mid - 1;
        }
    }
    return ans;
}

public static int countOccurrences(int[] arr, int target) {
    int first = firstOccurrence(arr, target);
    if (first == -1) return 0;
    int last = lastOccurrence(arr, target);
    return last - first + 1;
}



### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## C

### SOLUTION

int firstOccurrence(int arr[], int n, int target) {
    int low = 0, high = n - 1, ans = -1;
    while (low <= high) {
        int mid = low + (high - low) / 2;
        if (arr[mid] == target) {
            ans = mid;
            high = mid - 1;
        } else if (arr[mid] < target) {
            low = mid + 1;
        } else {
            high = mid - 1;
        }
    }
    return ans;
}

int lastOccurrence(int arr[], int n, int target) {
    int low = 0, high = n - 1, ans = -1;
    while (low <= high) {
        int mid = low + (high - low) / 2;
        if (arr[mid] == target) {
            ans = mid;
            low = mid + 1;
        } else if (arr[mid] < target) {
            low = mid + 1;
        } else {
            high = mid - 1;
        }
    }
    return ans;
}

int countOccurrences(int arr[], int n, int target) {
    int first = firstOccurrence(arr, n, target);
    if (first == -1) return 0;
    int last = lastOccurrence(arr, n, target);
    return last - first + 1;
}

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## JAVASCRIPT

### SOLUTION

function firstOccurrence(arr, target) {
    let low = 0, high = arr.length - 1, ans = -1;
    while (low <= high) {
        let mid = Math.floor(low + (high - low) / 2);
        if (arr[mid] === target) {
            ans = mid;
            high = mid - 1;
        } else if (arr[mid] < target) {
            low = mid + 1;
        } else {
            high = mid - 1;
        }
    }
    return ans;
}

function lastOccurrence(arr, target) {
    let low = 0, high = arr.length - 1, ans = -1;
    while (low <= high) {
        let mid = Math.floor(low + (high - low) / 2);
        if (arr[mid] === target) {
            ans = mid;
            low = mid + 1;
        } else if (arr[mid] < target) {
            low = mid + 1;
        } else {
            high = mid - 1;
        }
    }
    return ans;
}

function countOccurrences(arr, target) {
    const first = firstOccurrence(arr, target);
    if (first === -1) return 0;
    const last = lastOccurrence(arr, target);
    return last - first + 1;
}


### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## PYTHON

### SOLUTION


def firstOccurrence(arr: List[int], target: int) -> int:
    low, high, ans = 0, len(arr) - 1, -1
    while low <= high:
        mid = low + (high - low) // 2
        if arr[mid] == target:
            ans = mid
            high = mid - 1
        elif arr[mid] < target:
            low = mid + 1
        else:
            high = mid - 1
    return ans

def lastOccurrence(arr: List[int], target: int) -> int:
    low, high, ans = 0, len(arr) - 1, -1
    while low <= high:
        mid = low + (high - low) // 2
        if arr[mid] == target:
            ans = mid
            low = mid + 1
        elif arr[mid] < target:
            low = mid + 1
        else:
            high = mid - 1
    return ans

def countOccurrences(arr: List[int], target: int) -> int:
    first = firstOccurrence(arr, target)
    if first == -1:
        return 0
    last = lastOccurrence(arr, target)
    return last - first + 1

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256
