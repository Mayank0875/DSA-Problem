## CPP

### SOLUTION


int totalSolutions;
vector<bool> col;
vector<bool> diag1;
vector<bool> diag2;
int boardSize;

void solve(int y) {
    if (y == boardSize) {
        totalSolutions++;
        return;
    }
    for (int x = 0; x < boardSize; x++) {
        if (col[x] || diag1[x + y] || diag2[x - y + boardSize - 1]) {
            continue;
        }
        col[x] = diag1[x + y] = diag2[x - y + boardSize - 1] = true;
        solve(y + 1);
        col[x] = diag1[x + y] = diag2[x - y + boardSize - 1] = false;
    }
}

int countSolutions(int n) {
    totalSolutions = 0;
    boardSize = n;
    
    col.assign(n, false);
    diag1.assign(2 * n - 1, false);
    diag2.assign(2 * n - 1, false);
    
    solve(0);
    return totalSolutions;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

static int totalSolutions;
static boolean[] col;
static boolean[] diag1;
static boolean[] diag2;
static int boardSize;

public static void solve(int y) {
    if (y == boardSize) {
        totalSolutions++;
        return;
    }
    for (int x = 0; x < boardSize; x++) {
        if (col[x] || diag1[x + y] || diag2[x - y + boardSize - 1]) continue;

        col[x] = diag1[x + y] = diag2[x - y + boardSize - 1] = true;
        solve(y + 1);
        col[x] = diag1[x + y] = diag2[x - y + boardSize - 1] = false;
    }
}

public static int countSolutions(int n) {
    totalSolutions = 0;
    boardSize = n;

    col = new boolean[n];
    diag1 = new boolean[2 * n - 1];
    diag2 = new boolean[2 * n - 1];

    solve(0);
    return totalSolutions;
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

int totalSolutions;
bool col[30], diag1[60], diag2[60];
int boardSize;

void solve(int y) {
    if (y == boardSize) {
        totalSolutions++;
        return;
    }
    for (int x = 0; x < boardSize; x++) {
        if (col[x] || diag1[x + y] || diag2[x - y + boardSize - 1]) continue;

        col[x] = diag1[x + y] = diag2[x - y + boardSize - 1] = true;
        solve(y + 1);
        col[x] = diag1[x + y] = diag2[x - y + boardSize - 1] = false;
    }
}

int countSolutions(int n) {
    totalSolutions = 0;
    boardSize = n;

    for (int i = 0; i < n; i++) col[i] = false;
    for (int i = 0; i < 2 * n - 1; i++) diag1[i] = diag2[i] = false;

    solve(0);
    return totalSolutions;
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

let totalSolutions;
let col, diag1, diag2;
let boardSize;

function solve(y) {
    if (y === boardSize) {
        totalSolutions++;
        return;
    }
    for (let x = 0; x < boardSize; x++) {
        if (col[x] || diag1[x + y] || diag2[x - y + boardSize - 1]) continue;

        col[x] = diag1[x + y] = diag2[x - y + boardSize - 1] = true;
        solve(y + 1);
        col[x] = diag1[x + y] = diag2[x - y + boardSize - 1] = false;
    }
}

function countSolutions(n) {
    totalSolutions = 0;
    boardSize = n;

    col = new Array(n).fill(false);
    diag1 = new Array(2 * n - 1).fill(false);
    diag2 = new Array(2 * n - 1).fill(false);

    solve(0);
    return totalSolutions;
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

totalSolutions = 0
col = []
diag1 = []
diag2 = []
boardSize = 0

def solve(y):
    global totalSolutions, col, diag1, diag2, boardSize
    if y == boardSize:
        totalSolutions += 1
        return
    for x in range(boardSize):
        if col[x] or diag1[x + y] or diag2[x - y + boardSize - 1]:
            continue
        col[x] = diag1[x + y] = diag2[x - y + boardSize - 1] = True
        solve(y + 1)
        col[x] = diag1[x + y] = diag2[x - y + boardSize - 1] = False

def countSolutions(n):
    global totalSolutions, col, diag1, diag2, boardSize
    totalSolutions = 0
    boardSize = n
    col = [False] * n
    diag1 = [False] * (2 * n - 1)
    diag2 = [False] * (2 * n - 1)
    solve(0)
    return totalSolutions


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  