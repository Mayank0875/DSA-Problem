## CPP

### SOLUTION

vector<vector<char>> applyGravity(vector<vector<char>>& box) {
    int m = box.size();
    int n = box[0].size();

    for (int col = 0; col < n; col++) {
        int write = m - 1;

        for (int row = m - 1; row >= 0; row--) {
            if (box[row][col] == '*') {
                write = row - 1;
            }
            else if (box[row][col] == '#') {
                swap(box[row][col], box[write][col]);
                write--;
            }
        }
    }
    return box;
}



### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public char[][] applyGravity(char[][] box) {
    int m = box.length;
    int n = box[0].length;

    for (int col = 0; col < n; col++) {
        int write = m - 1;

        for (int row = m - 1; row >= 0; row--) {
            if (box[row][col] == '*') {
                write = row - 1;
            }
            else if (box[row][col] == '#') {
                char temp = box[row][col];
                box[row][col] = box[write][col];
                box[write][col] = temp;
                write--;
            }
        }
    }
    return box;
}



### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION


char** applyGravity(char** box, int boxSize, int* boxColSize,
                    int* returnSize, int** returnColumnSizes) {

    int m = boxSize;
    int n = boxColSize[0];

    // Return dimensions
    *returnSize = m;
    *returnColumnSizes = (int*)malloc(m * sizeof(int));

    char** result = (char**)malloc(m * sizeof(char*));
    for (int i = 0; i < m; i++) {
        (*returnColumnSizes)[i] = n;
        result[i] = (char*)malloc(n * sizeof(char));
        for (int j = 0; j < n; j++) {
            result[i][j] = box[i][j];
        }
    }

    // Apply gravity column-wise
    for (int col = 0; col < n; col++) {
        int write = m - 1;

        for (int row = m - 1; row >= 0; row--) {
            if (result[row][col] == '*') {
                write = row - 1;
            }
            else if (result[row][col] == '#') {
                char temp = result[row][col];
                result[row][col] = result[write][col];
                result[write][col] = temp;
                write--;
            }
        }
    }

    return result;
}



### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function applyGravity(box) {
    const m = box.length;
    const n = box[0].length;

    for (let col = 0; col < n; col++) {
        let write = m - 1;

        for (let row = m - 1; row >= 0; row--) {
            if (box[row][col] === '*') {
                write = row - 1;
            }
            else if (box[row][col] === '#') {
                [box[row][col], box[write][col]] =
                [box[write][col], box[row][col]];
                write--;
            }
        }
    }
    return box;
}



### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def applyGravity(box):
    m, n = len(box), len(box[0])

    for col in range(n):
        write = m - 1
        for row in range(m - 1, -1, -1):
            if box[row][col] == '*':
                write = row - 1
            elif box[row][col] == '#':
                box[row][col], box[write][col] = box[write][col], box[row][col]
                write -= 1
    return box



### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  