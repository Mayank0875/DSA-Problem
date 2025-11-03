## CPP

### SOLUTION

int Finder(vector<int>& keys, int target) {
    int low = 0, high = keys.size() - 1;
    while (low <= high) {
        int mid = low + (high - low) / 2;
        if (keys[mid] == target) {
            return mid;
        }
        if (keys[low] <= keys[mid]) {
            if (target >= keys[low] && target < keys[mid]) {
                high = mid - 1;
            } else {
                low = mid + 1;
            }
        }
        else {
            if (target > keys[mid] && target <= keys[high]) {
                low = mid + 1; 
            } else {
                high = mid - 1;
            }
        }
    }
    return -1; 
}


### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## JAVA

### SOLUTION

public static int Finder(int[] keys, int target) {
    int low = 0, high = keys.length - 1;
    while (low <= high) {
        int mid = low + (high - low) / 2;
        if (keys[mid] == target) {
            return mid;
        }
        if (keys[low] <= keys[mid]) { 
            if (target >= keys[low] && target < keys[mid]) {
                high = mid - 1;
            } else {
                low = mid + 1;
            }
        } else { 
            if (target > keys[mid] && target <= keys[high]) {
                low = mid + 1;
            } else {
                high = mid - 1;
            }
        }
    }
    return -1;
}



### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## C

### SOLUTION

int Finder(int arr[], int n, int target) {
    int low = 0, high = n - 1;
    while (low <= high) {
        int mid = low + (high - low) / 2;
        if (arr[mid] == target) {
            return mid;
        }
        if (arr[low] <= arr[mid]) { 
            if (target >= arr[low] && target < arr[mid]) {
                high = mid - 1;
            } else {
                low = mid + 1;
            }
        } else { 
            if (target > arr[mid] && target <= arr[high]) {
                low = mid + 1;
            } else {
                high = mid - 1;
            }
        }
    }
    return -1; 
}

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## JAVASCRIPT

### SOLUTION

function Finder(keys, target) {
    let low = 0, high = keys.length - 1;
    while (low <= high) {
        let mid = Math.floor(low + (high - low) / 2);
        if (keys[mid] === target) {
            return mid;
        }
        if (keys[low] <= keys[mid]) { 
            if (target >= keys[low] && target < keys[mid]) {
                high = mid - 1;
            } else {
                low = mid + 1;
            }
        } else { 
            if (target > keys[mid] && target <= keys[high]) {
                low = mid + 1;
            } else {
                high = mid - 1;
            }
        }
    }
    return -1; 
}


### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## PYTHON

### SOLUTION



def Finder(keys: List[int], target: int) -> int:
    low, high = 0, len(keys) - 1
    while low <= high:
        mid = low + (high - low) // 2
        if keys[mid] == target:
            return mid
        if keys[low] <= keys[mid]: 
            if target >= keys[low] and target < keys[mid]:
                high = mid - 1
            else:
                low = mid + 1
        else:  
            if target > keys[mid] and target <= keys[high]:
                low = mid + 1
            else:
                high = mid - 1
    return -1 

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256
