## CPP

### SOLUTION

bool asteroidsDestroyed(int mass, vector<int>& asteroids) {
    sort(asteroids.begin(), asteroids.end());

    long long res = mass;
    for(auto val : asteroids) {
        if(res < val) return false;
        res += val;
    }
    return true;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static boolean asteroidsDestroyed(int mass, int[] asteroids) {
    Arrays.sort(asteroids);
    
    long res = mass;
    for (int val : asteroids) {
        if (res < val) {
            return false;
        }
        res += val;
    }
    return true;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

int compare(const void* a, const void* b) {
    return (*(int*)a - *(int*)b);
}

bool asteroidsDestroyed(int mass, int* asteroids, int asteroidsSize) {
    qsort(asteroids, asteroidsSize, sizeof(int), compare);
    
    long long res = mass;
    for (int i = 0; i < asteroidsSize; i++) {
        if (res < asteroids[i]) {
            return false;
        }
        res += asteroids[i];
    }
    return true;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function asteroidsDestroyed(mass, asteroids) {
    asteroids.sort((a, b) => a - b);
    
    let res = mass;
    for (let val of asteroids) {
        if (res < val) {
            return false;
        }
        res += val;
    }
    return true;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def asteroidsDestroyed(mass: int, asteroids: list) -> bool:
    asteroids.sort()
    
    res = mass
    for val in asteroids:
        if res < val:
            return False
        res += val
    return True

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  