## CPP

### SOLUTION

bool canReachEnd(vector<int>& platforms) {
    int goal = platforms.size() - 1;

    for (int i = platforms.size() - 2; i >= 0; i--) {
        if (i + platforms[i] >= goal) {
            goal = i;
        }
    }

    return goal == 0;        
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static boolean canReachEnd(int[] platforms) {
    int goal = platforms.length - 1;

    for (int i = platforms.length - 2; i >= 0; i--) {
        if (i + platforms[i] >= goal) {
            goal = i;
        }
    }

    return goal == 0;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

bool canReachEnd(int* platforms, int platformsSize) {
    int goal = platformsSize - 1;

    for (int i = platformsSize - 2; i >= 0; i--) {
        if (i + platforms[i] >= goal) {
            goal = i;
        }
    }

    return goal == 0;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function canReachEnd(platforms) {
    let goal = platforms.length - 1;

    for (let i = platforms.length - 2; i >= 0; i--) {
        if (i + platforms[i] >= goal) {
            goal = i;
        }
    }

    return goal === 0;    
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION


def canReachEnd(platforms: list) -> bool:
    goal = len(platforms) - 1

    for i in range(len(platforms) - 2, -1, -1):
        if i + platforms[i] >= goal:
            goal = i
    
    return True if goal == 0 else False

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  