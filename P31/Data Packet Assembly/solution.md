## CPP

### SOLUTION


void solve(int target, vector<int>& candidates, int startIndex, int& count) {
    if (target == 0) {
        count++;
        return;
    }
    if (target < 0) {
        return;
    }
    
    for (int i = startIndex; i < candidates.size(); ++i) {
        if (i > startIndex && candidates[i] == candidates[i-1]) {
            continue;
        }
        
        if (target - candidates[i] < 0) {
            break;
        }
        
        solve(target - candidates[i], candidates, i + 1, count);
    }
}

int countUniqueCombinations(vector<int>& candidates, int target) {
    sort(candidates.begin(), candidates.end());
    int count = 0;
    solve(target, candidates, 0, count);
    return count;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

static void solve(int target, int[] candidates, int startIndex, int[] count) {
    if (target == 0) {
        count[0]++;
        return;
    }
    if (target < 0) return;

    for (int i = startIndex; i < candidates.length; i++) {
        if (i > startIndex && candidates[i] == candidates[i - 1]) continue;
        if (target - candidates[i] < 0) break;

        solve(target - candidates[i], candidates, i + 1, count);
    }
}

public static int countUniqueCombinations(int[] candidates, int target) {
    Arrays.sort(candidates);
    int[] count = new int[1];
    solve(target, candidates, 0, count);
    return count[0];
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

void solve(int target, int* candidates, int size, int startIndex, int* count) {
    if (target == 0) {
        (*count)++;
        return;
    }
    if (target < 0) return;

    for (int i = startIndex; i < size; i++) {
        if (i > startIndex && candidates[i] == candidates[i - 1]) continue;
        if (target - candidates[i] < 0) break;

        solve(target - candidates[i], candidates, size, i + 1, count);
    }
}

int cmp(const void* a, const void* b) {
    return (*(int*)a - *(int*)b);
}

int countUniqueCombinations(int* candidates, int size, int target) {
    qsort(candidates, size, sizeof(int), cmp);
    int count = 0;
    solve(target, candidates, size, 0, &count);
    return count;
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function solve(target, candidates, startIndex, count) {
    if (target === 0) {
        count.value++;
        return;
    }
    if (target < 0) return;

    for (let i = startIndex; i < candidates.length; i++) {
        if (i > startIndex && candidates[i] === candidates[i - 1]) continue;
        if (target - candidates[i] < 0) break;

        solve(target - candidates[i], candidates, i + 1, count);
    }
}

function countUniqueCombinations(candidates, target) {
    candidates.sort((a, b) => a - b);
    const count = { value: 0 };
    solve(target, candidates, 0, count);
    return count.value;
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def solve(target, candidates, start_index, count):
    if target == 0:
        count[0] += 1
        return
    if target < 0:
        return

    for i in range(start_index, len(candidates)):
        if i > start_index and candidates[i] == candidates[i - 1]:
            continue
        if target - candidates[i] < 0:
            break

        solve(target - candidates[i], candidates, i + 1, count)

def countUniqueCombinations(candidates, target):
    candidates.sort()
    count = [0]
    solve(target, candidates, 0, count)
    return count[0]


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  