## CPP

### SOLUTION

string solveGame(int n, vector<int>& a, vector<int>& b) {
    int score = 0;
    int different_idx = -1;
    
    for(int i = 0; i < n; ++i) {
        if(a[i] != b[i]) {
            different_idx = i + 1;
        }
        score ^= a[i];
        score ^= b[i];
    }

    if(score != 0) {
        if (different_idx & 1) return "Alex";
        else return "Sam";
    } else {
        return "Tie";
    }
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static String solveGame(int n, int[] a, int[] b) {
    int score = 0;
    int differentIdx = -1;

    for (int i = 0; i < n; i++) {
        if (a[i] != b[i]) {
            differentIdx = i + 1;
        }
        score ^= a[i];
        score ^= b[i];
    }

    if (score != 0) {
        if ((differentIdx & 1) == 1) return "Alex";
        else return "Sam";
    } else {
        return "Tie";
    }
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

char* solveGame(int n, int* a, int* b) {
    int score = 0;
    int different_idx = -1;

    for(int i = 0; i < n; ++i) {
        if(a[i] != b[i]) {
            different_idx = i + 1;
        }
        score ^= a[i];
        score ^= b[i];
    }

    if(score != 0) {
        char* res = (char*)malloc(5 * sizeof(char));
        if (different_idx & 1) strcpy(res, "Alex");
        else strcpy(res, "Sam");
        return res;
    } else {
        char* res = (char*)malloc(4 * sizeof(char));
        strcpy(res, "Tie");
        return res;
    }
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function solveGame(n, a, b) {
    let score = 0;
    let differentIdx = -1;

    for(let i = 0; i < n; ++i) {
        if(a[i] !== b[i]) {
            differentIdx = i + 1;
        }
        score ^= a[i];
        score ^= b[i];
    }

    if(score !== 0) {
        if (differentIdx & 1) return "Alex";
        else return "Sam";
    } else {
        return "Tie";
    }
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def solveGame(n: int, a: list, b: list) -> str:
    score = 0
    different_idx = -1
    
    for i in range(n):
        if a[i] != b[i]:
            different_idx = i + 1
        score ^= a[i]
        score ^= b[i]
        
    if score != 0:
        if different_idx & 1:
            return "Alex"
        else:
            return "Sam"
    else:
        return "Tie"

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  