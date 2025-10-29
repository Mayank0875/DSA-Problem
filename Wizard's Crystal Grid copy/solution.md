## CPP

### SOLUTION

int findMissingItem(int n, vector<int>& present_items) {
    long long expected_sum = (long long)n * (n + 1) / 2;
    long long actual_sum = 0;
    for (int item : present_items) {
        actual_sum += item;
    }
    return expected_sum - actual_sum;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static long findMissingItem(int n, int[] present_items) {
    long expected_sum = (long)n * (n + 1) / 2;
    long actual_sum = 0;
    for (int item : present_items) {
        actual_sum += item;
    }
    return expected_sum - actual_sum;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

long long findMissingItem(int n, int present_items[], int size) {
    long long expected_sum = (long long)n * (n + 1) / 2;
    long long actual_sum = 0;
    for (int i = 0; i < size; i++) {
        actual_sum += present_items[i];
    }
    return expected_sum - actual_sum;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function findMissingItem(n, present_items) {
    let expected_sum = BigInt(n) * BigInt(n + 1) / 2n;
    let actual_sum = 0n;
    for (let item of present_items) {
        actual_sum += BigInt(item);
    }
    return expected_sum - actual_sum;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def findMissingItem(n, present_items):
    expected_sum = n * (n + 1) // 2
    actual_sum = sum(present_items)
    return expected_sum - actual_sum

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  