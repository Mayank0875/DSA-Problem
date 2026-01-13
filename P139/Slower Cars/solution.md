## CPP

### SOLUTION

int numberOfWeakCharacters(vector<vector<int>>& properties) {
    sort(properties.begin(), properties.end(), [](const vector<int>& a, const vector<int>& b) {
        if (a[0] == b[0]) {
            return a[1] < b[1];
        }
        return a[0] > b[0];
    });

    int maxDefense = INT_MIN;
    int count = 0;

    for (const auto& p : properties) {
        if (p[1] < maxDefense) {
            count++;
        }
        maxDefense = max(maxDefense, p[1]);
    }

    return count;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static int numberOfWeakCharacters(int[][] properties) {
    // Sort by attack descending. If attack is same, sort by defense ascending.
    Arrays.sort(properties, (a, b) -> {
        if (a[0] == b[0]) {
            return Integer.compare(a[1], b[1]);
        }
        return Integer.compare(b[0], a[0]);
    });

    int maxDefense = Integer.MIN_VALUE;
    int count = 0;

    for (int[] p : properties) {
        if (p[1] < maxDefense) {
            count++;
        }
        maxDefense = Math.max(maxDefense, p[1]);
    }

    return count;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

// Comparator function for qsort
int compare(const void* a, const void* b) {
    int* p1 = *(int**)a;
    int* p2 = *(int**)b;
    
    // Sort by attack descending
    if (p1[0] != p2[0]) {
        return p2[0] - p1[0];
    }
    // If attacks are equal, sort by defense ascending
    return p1[1] - p2[1];
}

int numberOfWeakCharacters(int** properties, int propertiesSize, int* propertiesColSize) {
    qsort(properties, propertiesSize, sizeof(int*), compare);

    int maxDefense = INT_MIN;
    int count = 0;

    for (int i = 0; i < propertiesSize; i++) {
        if (properties[i][1] < maxDefense) {
            count++;
        }
        if (properties[i][1] > maxDefense) {
            maxDefense = properties[i][1];
        }
    }

    return count;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function numberOfWeakCharacters(properties) {
    // Sort: Attack Descending, Defense Ascending
    properties.sort((a, b) => {
        if (a[0] === b[0]) {
            return a[1] - b[1];
        }
        return b[0] - a[0];
    });

    let maxDefense = -Infinity;
    let count = 0;

    for (const p of properties) {
        if (p[1] < maxDefense) {
            count++;
        }
        maxDefense = Math.max(maxDefense, p[1]);
    }

    return count;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def numberOfWeakCharacters(properties: list) -> int:
    # Sort by attack descending (-x[0]), then defense ascending (x[1])
    properties.sort(key=lambda x: (-x[0], x[1]))
    
    max_defense = float('-inf')
    count = 0
    
    for _, defense in properties:
        if defense < max_defense:
            count += 1
        else:
            max_defense = defense
            
    return count

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  