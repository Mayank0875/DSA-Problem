## CPP

### SOLUTION

string hasDuplicateIDs(vector<int>& ids) {
    sort(ids.begin(), ids.end());
    for (int i = 0; i < ids.size() - 1; ++i) {
        if (ids[i] == ids[i + 1]) {
            return "Yes";
        }
    }
    return "No";
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static String hasDuplicateIDs(List<Integer> ids) {
    Collections.sort(ids);
    for (int i = 0; i < ids.size() - 1; i++) {
        if (ids.get(i).equals(ids.get(i + 1))) {
            return "Yes";
        }
    }
    return "No";
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION


char* hasDuplicateIDs(int* ids, int size) {
    qsort(ids, size, sizeof(int), compare);
    for (int i = 0; i < size - 1; i++) {
        if (ids[i] == ids[i + 1]) {
            return "Yes";
        }
    }
    return "No";
}

int compare(const void* a, const void* b) {
    return (*(int*)a - *(int*)b);
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function hasDuplicateIDs(ids) {
    ids.sort((a, b) => a - b);
    for (let i = 0; i < ids.length - 1; i++) {
        if (ids[i] === ids[i + 1]) {
            return "Yes";
        }
    }
    return "No";
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def hasDuplicateIDs(ids):
    ids.sort()
    for i in range(len(ids) - 1):
        if ids[i] == ids[i + 1]:
            return "Yes"
    return "No"

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  