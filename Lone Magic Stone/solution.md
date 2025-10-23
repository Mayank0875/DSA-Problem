## CPP

### SOLUTION

int findLoneStone(vector<int>& stones) {
    int left = 0, right = stones.size() - 1;
    while (left < right) {
        int mid = left + (right - left) / 2;
        if (mid % 2 == 1) {
            mid--; 
        }
        if (stones[mid] == stones[mid + 1]) {
            left = mid + 2;
        } 
        else {
            right = mid;
        }
    }
    return stones[left];
}


### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## JAVA

### SOLUTION

public static int findLoneStone(int[] stones) {
    int left = 0, right = stones.length - 1;
    while (left < right) {
        int mid = left + (right - left) / 2;
        if (mid % 2 == 1) {
            mid--;
        }
        if (stones[mid] == stones[mid + 1]) {
            left = mid + 2;
        } else {
            right = mid;
        }
    }
    return stones[left];
}



### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## C

### SOLUTION

int findLoneStone(int stones[], int n) {
    int left = 0, right = n - 1;
    while (left < right) {
        int mid = left + (right - left) / 2;
        if (mid % 2 == 1) {
            mid--;
        }
        if (stones[mid] == stones[mid + 1]) {
            left = mid + 2;
        } else {
            right = mid;
        }
    }
    return stones[left];
}

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## JAVASCRIPT

### SOLUTION

function findLoneStone(stones) {
    let left = 0, right = stones.length - 1;
    while (left < right) {
        let mid = Math.floor(left + (right - left) / 2);
        if (mid % 2 === 1) {
            mid--;
        }
        if (stones[mid] === stones[mid + 1]) {
            left = mid + 2;
        } else {
            right = mid;
        }
    }
    return stones[left];
}


### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## PYTHON

### SOLUTION

def findLoneStone(stones: list[int]) -> int:
    left, right = 0, len(stones) - 1
    while left < right:
        mid = left + (right - left) // 2
        if mid % 2 == 1:
            mid -= 1
        if stones[mid] == stones[mid + 1]:
            left = mid + 2
        else:
            right = mid
    return stones[left]

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256
