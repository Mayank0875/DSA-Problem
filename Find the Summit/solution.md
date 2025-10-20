## CPP

### SOLUTION

int findPeakElementIndex(vector<int>& arr) {
    int left = 0;
    int right = arr.size() - 1;

    while (left < right) {
        int mid = left + (right - left) / 2;
        if (arr[mid] < arr[mid + 1]) {
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
    public static int findPeakElementIndex(int[] arr) {
        int left = 0;
        int right = arr.length - 1;

        while (left < right) {
            int mid = left + (right - left) / 2;
            if (arr[mid] < arr[mid + 1]) {
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

int findPeakElementIndex(int arr[], int n) {
    int left = 0;
    int right = n - 1;

    while (left < right) {
        int mid = left + (right - left) / 2;
        if (arr[mid] < arr[mid + 1]) {
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

function findPeakElementIndex(arr) {
    let left = 0;
    let right = arr.length - 1;

    while (left < right) {
        let mid = Math.floor(left + (right - left) / 2);
        if (arr[mid] < arr[mid + 1]) {
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

def findPeakElementIndex(arr):
    left = 0
    right = len(arr) - 1

    while left < right:
        mid = left + (right - left) // 2
        if arr[mid] < arr[mid + 1]:
            left = mid + 1
        else:
            right = mid
    return left


### METADATA

**TimeLimit**
2000

**MemoryLimit**
256
