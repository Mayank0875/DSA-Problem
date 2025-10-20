## CPP

### SOLUTION

bool searchMatrix(vector<vector<int>>& matrix, int target) {
    if (matrix.empty() || matrix[0].empty()) {
        return false;
    }
    int m = matrix.size();
    int n = matrix[0].size();
    int left = 0;
    int right = m * n - 1;

    while (left <= right) {
        int mid = left + (right - left) / 2;
        int row = mid / n;
        int col = mid % n;
        int midVal = matrix[row][col];

        if (midVal == target) {
            return true;
        } else if (midVal < target) {
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
    public static boolean searchMatrix(int[][] matrix, int target) {
        if (matrix.length == 0 || matrix[0].length == 0) {
            return false;
        }

        int m = matrix.length;
        int n = matrix[0].length;
        int left = 0, right = m * n - 1;

        while (left <= right) {
            int mid = left + (right - left) / 2;
            int row = mid / n;
            int col = mid % n;
            int midVal = matrix[row][col];

            if (midVal == target) {
                return true;
            } else if (midVal < target) {
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

#include <stdbool.h>

bool searchMatrix(int** matrix, int m, int n, int target) {
    if (m == 0 || n == 0) {
        return false;
    }

    int left = 0, right = m * n - 1;

    while (left <= right) {
        int mid = left + (right - left) / 2;
        int row = mid / n;
        int col = mid % n;
        int midVal = matrix[row][col];

        if (midVal == target) {
            return true;
        } else if (midVal < target) {
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

function searchMatrix(matrix, target) {
    if (matrix.length === 0 || matrix[0].length === 0) {
        return false;
    }

    const m = matrix.length;
    const n = matrix[0].length;
    let left = 0, right = m * n - 1;

    while (left <= right) {
        const mid = Math.floor(left + (right - left) / 2);
        const row = Math.floor(mid / n);
        const col = mid % n;
        const midVal = matrix[row][col];

        if (midVal === target) {
            return true;
        } else if (midVal < target) {
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

def searchMatrix(matrix: List[List[int]], target: int) -> bool:
    if not matrix or not matrix[0]:
        return False

    m, n = len(matrix), len(matrix[0])
    left, right = 0, m * n - 1

    while left <= right:
        mid = left + (right - left) // 2
        row, col = divmod(mid, n)
        midVal = matrix[row][col]

        if midVal == target:
            return True
        elif midVal < target:
            left = mid + 1
        else:
            right = mid - 1

    return False

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256
