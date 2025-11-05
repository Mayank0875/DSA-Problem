## CPP

### SOLUTION

int solve(int target, vector<int>& candidates, int startIndex) {
    if (target == 0) {
        return 1;
    }
    if (target < 0) {
        return 0;
    }
    
    int count = 0;
    for (int i = startIndex; i < candidates.size(); ++i) {
        count += solve(target - candidates[i], candidates, i);
    }
    return count;
}

int countCombinations(vector<int>& candidates, int target) {
    return solve(target, candidates, 0);
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

static int solve(int target, int[] candidates, int startIndex) {
    if (target == 0) {
        return 1;
    }
    if (target < 0) {
        return 0;
    }

    int count = 0;
    for (int i = startIndex; i < candidates.length; i++) {
        count += solve(target - candidates[i], candidates, i);
    }
    return count;
}

public static int countCombinations(int[] candidates, int target) {
    return solve(target, candidates, 0);
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

int solve(int target, int* candidates, int size, int startIndex) {
    if (target == 0) {
        return 1;
    }
    if (target < 0) {
        return 0;
    }

    int count = 0;
    for (int i = startIndex; i < size; i++) {
        count += solve(target - candidates[i], candidates, size, i);
    }
    return count;
}

int countCombinations(int* candidates, int size, int target) {
    return solve(target, candidates, size, 0);
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function solve(target, candidates, startIndex) {
    if (target === 0) {
        return 1;
    }
    if (target < 0) {
        return 0;
    }

    let count = 0;
    for (let i = startIndex; i < candidates.length; i++) {
        count += solve(target - candidates[i], candidates, i);
    }
    return count;
}

function countCombinations(candidates, target) {
    return solve(target, candidates, 0);
}



### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def solve(target, candidates, startIndex):
    if target == 0:
        return 1
    if target < 0:
        return 0

    count = 0
    for i in range(startIndex, len(candidates)):
        count += solve(target - candidates[i], candidates, i)
    return count

def countCombinations(candidates, target):
    return solve(target, candidates, 0)


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  