## CPP

### SOLUTION

int solveFerrisWheel(int n, int x, vector<int>& p) {
    sort(p.begin(), p.end());
    int gondolas = 0;
    int i = 0;
    int j = n - 1;
    while (i <= j) {
        if (i != j && (long long)p[i] + p[j] <= x) {
            i++;
            j--;
        } else {
            j--;
        }
        gondolas++; 
    }
    return gondolas;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static int solveFerrisWheel(int n, int x, int[] p) {
    Arrays.sort(p);
    int gondolas = 0;
    int i = 0;
    int j = n - 1;

    while (i <= j) {
        if (i != j && (long)p[i] + p[j] <= x) {
            i++;
            j--;
        } else {
            j--;
        }
        gondolas++;
    }
    return gondolas;
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

int solveFerrisWheel(int n, int x, int* p) {
    qsort(p, n, sizeof(int), compare);

    int gondolas = 0;
    int i = 0;
    int j = n - 1;

    while (i <= j) {
        if (i != j && (long long)p[i] + p[j] <= x) {
            i++;
            j--;
        } else {
            j--;
        }
        gondolas++;
    }
    return gondolas;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function solveFerrisWheel(n, x, p) {
    p.sort((a, b) => a - b);
    let gondolas = 0;
    let i = 0;
    let j = n - 1;

    while (i <= j) {
        if (i !== j && p[i] + p[j] <= x) {
            i++;
            j--;
        } else {
            j--;
        }
        gondolas++;
    }
    return gondolas;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def solveFerrisWheel(n, x, p):
    p.sort()
    gondolas = 0
    i, j = 0, n - 1

    while i <= j:
        if i != j and p[i] + p[j] <= x:
            i += 1
            j -= 1
        else:
            j -= 1
        gondolas += 1

    return gondolas

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  