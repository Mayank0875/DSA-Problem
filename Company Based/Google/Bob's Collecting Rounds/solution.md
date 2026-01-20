## CPP

### SOLUTION

int countRounds(std::vector<int>& nums) {
    int n = nums.size();
    std::vector<int> pos(n + 1);
    
    // Store the position (index) of each number
    for (int i = 0; i < n; ++i) {
        pos[nums[i]] = i;
    }
    
    int rounds = 1;
    // Check transitions between consecutive numbers
    for (int i = 2; i <= n; ++i) {
        // If the position of (i) is before (i-1), we need a new round
        if (pos[i - 1] > pos[i]) {
            rounds++;
        }
    }
    
    return rounds;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public int countRounds(int[] nums) {
    int n = nums.length;
    int[] pos = new int[n + 1];
    
    for (int i = 0; i < n; i++) {
        pos[nums[i]] = i;
    }
    
    int rounds = 1;
    for (int i = 2; i <= n; i++) {
        if (pos[i - 1] > pos[i]) {
            rounds++;
        }
    }
    
    return rounds;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

int countRounds(int* nums, int numsSize) {
    int* pos = (int*)malloc((numsSize + 1) * sizeof(int));
    
    for (int i = 0; i < numsSize; i++) {
        pos[nums[i]] = i;
    }
    
    int rounds = 1;
    for (int i = 2; i <= numsSize; i++) {
        if (pos[i - 1] > pos[i]) {
            rounds++;
        }
    }
    
    free(pos);
    return rounds;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function countRounds(nums) {
    const n = nums.length;
    const pos = new Int32Array(n + 1);
    
    for (let i = 0; i < n; i++) {
        pos[nums[i]] = i;
    }
    
    let rounds = 1;
    for (let i = 2; i <= n; i++) {
        if (pos[i - 1] > pos[i]) {
            rounds++;
        }
    }
    
    return rounds;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def countRounds(nums):
    n = len(nums)
    pos = [0] * (n + 1)
    
    for i in range(n):
        pos[nums[i]] = i
        
    rounds = 1
    for i in range(2, n + 1):
        if pos[i - 1] > pos[i]:
            rounds += 1
            
    return rounds

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  