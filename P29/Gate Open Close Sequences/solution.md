## CPP

### SOLUTION

int backtrack(int openN, int closedN, int n) {
    if (openN == n && closedN == n) {
        return 1;
    }
    
    int count = 0;
    if (openN < n) {
        count += backtrack(openN + 1, closedN, n);
    }
    if (closedN < openN) {
        count += backtrack(openN, closedN + 1, n);
    }
    return count;
}

int countWellFormed(int n) {
    return backtrack(0, 0, n);
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

static int backtrack(int openN, int closedN, int n) {
    if (openN == n && closedN == n) {
        return 1;
    }

    int count = 0;
    if (openN < n) {
        count += backtrack(openN + 1, closedN, n);
    }
    if (closedN < openN) {
        count += backtrack(openN, closedN + 1, n);
    }
    return count;
}

public static int countWellFormed(int n) {
    return backtrack(0, 0, n);
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

int backtrack(int openN, int closedN, int n) {
    if (openN == n && closedN == n) {
        return 1;
    }

    int count = 0;
    if (openN < n) {
        count += backtrack(openN + 1, closedN, n);
    }
    if (closedN < openN) {
        count += backtrack(openN, closedN + 1, n);
    }
    return count;
}

int countWellFormed(int n) {
    return backtrack(0, 0, n);
}



### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function backtrack(openN, closedN, n) {
    if (openN === n && closedN === n) {
        return 1;
    }

    let count = 0;
    if (openN < n) {
        count += backtrack(openN + 1, closedN, n);
    }
    if (closedN < openN) {
        count += backtrack(openN, closedN + 1, n);
    }
    return count;
}

function countWellFormed(n) {
    return backtrack(0, 0, n);
}



### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def backtrack(openN, closedN, n):
    if openN == n and closedN == n:
        return 1

    count = 0
    if openN < n:
        count += backtrack(openN + 1, closedN, n)
    if closedN < openN:
        count += backtrack(openN, closedN + 1, n)
    return count

def countWellFormed(n):
    return backtrack(0, 0, n)



### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  