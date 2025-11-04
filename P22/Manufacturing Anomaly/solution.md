## CPP

### SOLUTION

int findVal(vector<int>& arr) {
    int left = 0, right = arr.size() - 1;
    while (left < right) {
        int mid = left + (right - left) / 2;
        if (mid % 2 == 1) {
            mid--; 
        }
        if (arr[mid] == arr[mid + 1]) {
            left = mid + 2;
        } 
        else {
            right = mid;
        }
    }
    return arr[left];
}


### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## JAVA

### SOLUTION

public static int findVal(int[] arr) {
    int left = 0, right = arr.length - 1;
    while (left < right) {
        int mid = left + (right - left) / 2;
        if (mid % 2 == 1) {
            mid--;
        }
        if (arr[mid] == arr[mid + 1]) {
            left = mid + 2;
        } else {
            right = mid;
        }
    }
    return arr[left];
}



### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## C

### SOLUTION

int findVal(int arr[], int n) {
    int left = 0, right = n - 1;
    while (left < right) {
        int mid = left + (right - left) / 2;
        if (mid % 2 == 1) {
            mid--;
        }
        if (arr[mid] == arr[mid + 1]) {
            left = mid + 2;
        } else {
            right = mid;
        }
    }
    return arr[left];
}

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## JAVASCRIPT

### SOLUTION

function findVal(arr) {
    let left = 0, right = arr.length - 1;
    while (left < right) {
        let mid = Math.floor(left + (right - left) / 2);
        if (mid % 2 === 1) {
            mid--;
        }
        if (arr[mid] === arr[mid + 1]) {
            left = mid + 2;
        } else {
            right = mid;
        }
    }
    return arr[left];
}


### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## PYTHON

### SOLUTION

def findVal(arr: list[int]) -> int:
    left, right = 0, len(arr) - 1
    while left < right:
        mid = left + (right - left) // 2
        if mid % 2 == 1:
            mid -= 1
        if arr[mid] == arr[mid + 1]:
            left = mid + 2
        else:
            right = mid
    return arr[left]

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256
