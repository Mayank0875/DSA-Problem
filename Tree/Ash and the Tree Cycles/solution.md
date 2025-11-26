## CPP

### SOLUTION

int Mininum_Edges(vector<vector<int>> &edges) {
    int n = edges.size() + 1;
    int res = ((n - 1) / 2);
    return res;
}

### METADATA

**TimeLimit**
1000

**MemoryLimit**
512



## JAVA

### SOLUTION

public static int Mininum_Edges(List<List<Integer>> edges) {
    int n = edges.size() + 1;
    int res = (n - 1) / 2;
    return res;
}

### METADATA

**TimeLimit**
1000

**MemoryLimit**
512



## C

### SOLUTION

int Mininum_Edges(int** edges, int edgesSize) {
    int n = edgesSize + 1;
    int res = (n - 1) / 2;
    return res;
}

### METADATA

**TimeLimit**
1000

**MemoryLimit**
512



## JAVASCRIPT

### SOLUTION

function Mininum_Edges(edges) {
    const n = edges.length + 1;
    const res = Math.floor((n - 1) / 2);
    return res;
}

### METADATA

**TimeLimit**
1000

**MemoryLimit**
512



## PYTHON

### SOLUTION


def Mininum_Edges(edges):
    n = len(edges) + 1
    res = (n - 1) // 2
    return res

### METADATA

**TimeLimit**
1000

**MemoryLimit**
512