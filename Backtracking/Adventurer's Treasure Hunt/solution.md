## CPP

### SOLUTION

bool solve(const vector<long long>& arr, int n, int index, long long remaining_sum) {
    if (remaining_sum == 0) {
        return true;
    }
    
    if (index == n || remaining_sum < 0) {
        return false;
    }
    
    if (solve(arr, n, index + 1, remaining_sum)) {
        return true;
    }
    
    if (solve(arr, n, index + 1, remaining_sum - arr[index])) {
        return true;
    }
    
    return false;
}

bool hasSubsetSum(vector<long long>& arr, long long sum) {
    int n = arr.size();
    return solve(arr, n, 0, sum);
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static boolean solve(long[] arr, int n, int index, long remaining_sum) {
    if (remaining_sum == 0)
        return true;

    if (index == n || remaining_sum < 0)
        return false;

    if (solve(arr, n, index + 1, remaining_sum))
        return true;

    if (solve(arr, n, index + 1, remaining_sum - arr[index]))
        return true;

    return false;
}

public static boolean hasSubsetSum(long[] arr, long sum) {
    int n = arr.length;
    return solve(arr, n, 0, sum);
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION


bool solve(long long* arr, int n, int index, long long remaining_sum) {
    if (remaining_sum == 0)
        return true;

    if (index == n || remaining_sum < 0)
        return false;

    if (solve(arr, n, index + 1, remaining_sum))
        return true;

    if (solve(arr, n, index + 1, remaining_sum - arr[index]))
        return true;

    return false;
}

bool hasSubsetSum(long long* arr, int n, long long sum) {
    return solve(arr, n, 0, sum);
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function solve(arr, n, index, remaining_sum) {
    if (remaining_sum === 0)
        return true;

    if (index === n || remaining_sum < 0)
        return false;

    if (solve(arr, n, index + 1, remaining_sum))
        return true;

    if (solve(arr, n, index + 1, remaining_sum - arr[index]))
        return true;

    return false;
}

function hasSubsetSum(arr, sum) {
    const n = arr.length;
    return solve(arr, n, 0, sum);
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def solve(arr, n, index, remaining_sum):
    if remaining_sum == 0:
        return True

    if index == n or remaining_sum < 0:
        return False

    if solve(arr, n, index + 1, remaining_sum):
        return True

    if solve(arr, n, index + 1, remaining_sum - arr[index]):
        return True

    return False


def hasSubsetSum(arr, total_sum):
    n = len(arr)
    return solve(arr, n, 0, total_sum)


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  