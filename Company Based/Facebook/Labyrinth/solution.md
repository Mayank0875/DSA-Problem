## CPP

### SOLUTION

vector<vector<char>> rotateTheBox(vector<vector<char>>& box) {
    int m = box.size();
    int n = box[0].size();
    vector<vector<char>> result(n, vector<char>(m, '.'));

    for (int i = 0; i < m; i++) {
        int lowestRowWithEmptyCell = n - 1;
        for (int j = n - 1; j >= 0; j--) {
            if (box[i][j] == '#') {
                // Place it in the correct position in the rotated grid
                result[lowestRowWithEmptyCell][m - i - 1] = '#';
                lowestRowWithEmptyCell--;
            }
            if (box[i][j] == '*') {
                result[j][m - i - 1] = '*';
                lowestRowWithEmptyCell = j - 1;
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


## JAVA

### SOLUTION

public char[][] rotateTheBox(char[][] box) {
    int m = box.length;
    int n = box[0].length;
    char[][] result = new char[n][m];

    for (int i = 0; i < n; i++) {
        for (int j = 0; j < m; j++) {
            result[i][j] = '.';
        }
    }

    for (int i = 0; i < m; i++) {
        int lowestRowWithEmptyCell = n - 1;
        for (int j = n - 1; j >= 0; j--) {
            if (box[i][j] == '#') {
                // Place it in the correct position in the rotated grid
                result[lowestRowWithEmptyCell][m - i - 1] = '#';
                lowestRowWithEmptyCell--;
            }
            if (box[i][j] == '*') {
                result[j][m - i - 1] = '*';
                lowestRowWithEmptyCell = j - 1;
            }
        }
    }
    return result;
}

### METADATA

**TimeLimit**  
3200  

**MemoryLimit**  
512  



## C

### SOLUTION


char** rotateTheBox(char** box, int boxSize, int* boxColSize, int* returnSize, int** returnColumnSizes) {
    int m = boxSize;
    int n = boxColSize[0];
    
    *returnSize = n;
    *returnColumnSizes = (int*)malloc(n * sizeof(int));
    char** result = (char**)malloc(n * sizeof(char*));
    
    for(int i = 0; i < n; i++) {
        (*returnColumnSizes)[i] = m;
        result[i] = (char*)malloc(m * sizeof(char));
        for(int j = 0; j < m; j++) {
            result[i][j] = '.';
        }
    }

    for(int i = 0; i < m; i++) {
        int lowestRowWithEmptyCell = n - 1;
        for(int j = n - 1; j >= 0; j--) {
            if(box[i][j] == '#') {
                result[lowestRowWithEmptyCell][m - i - 1] = '#';
                lowestRowWithEmptyCell--;
            }
            if(box[i][j] == '*') {
                result[j][m - i - 1] = '*';
                lowestRowWithEmptyCell = j - 1;
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

var rotateTheBox = function(box) {
    let m = box.length;
    let n = box[0].length;
    let result = Array.from({length: n}, () => Array(m).fill('.'));

    for (let i = 0; i < m; i++) {
        let lowestRowWithEmptyCell = n - 1;
        for (let j = n - 1; j >= 0; j--) {
            if (box[i][j] === '#') {
                result[lowestRowWithEmptyCell][m - i - 1] = '#';
                lowestRowWithEmptyCell--;
            }
            if (box[i][j] === '*') {
                result[j][m - i - 1] = '*';
                lowestRowWithEmptyCell = j - 1;
            }
        }
    }
    return result;
};

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def rotateTheBox(box: list) -> list:
    m = len(box)
    n = len(box[0])
    result = [["." for _ in range(m)] for _ in range(n)]

    for i in range(m):
        lowest_row_with_empty_cell = n - 1
        for j in range(n - 1, -1, -1):
            if box[i][j] == "#":
                result[lowest_row_with_empty_cell][m - i - 1] = "#"
                lowest_row_with_empty_cell -= 1
            if box[i][j] == "*":
                # Place the obstacle in the correct position in the rotated grid
                result[j][m - i - 1] = "*"
                lowest_row_with_empty_cell = j - 1

    return result

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  
