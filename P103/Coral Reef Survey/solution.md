## CPP

### SOLUTION

int numIslands(vector<vector<char>>& grid) {
    int islands = 0;
    int rows = grid.size();
    if (rows == 0) return 0;
    int cols = grid[0].size();

    for (int r = 0; r < rows; r++) {
        for (int c = 0; c < cols; c++) {
            if (grid[r][c] == '1') {
                islands++;
                // BFS to mark the entire island
                queue<pair<int, int>> q;
                q.push({r, c});
                grid[r][c] = '0';

                vector<pair<int, int>> directions = {{1, 0}, {-1, 0}, {0, 1}, {0, -1}};

                while (!q.empty()) {
                    auto [row, col] = q.front();
                    q.pop();

                    for (auto [dr, dc] : directions) {
                        int nr = row + dr;
                        int nc = col + dc;
                        if (nr >= 0 && nr < rows && nc >= 0 && nc < cols && grid[nr][nc] == '1') {
                            q.push({nr, nc});
                            grid[nr][nc] = '0'; // Mark as visited
                        }
                    }
                }
            }
        }
    }

    return islands;        
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public int numIslands(char[][] grid) {
    if (grid == null || grid.length == 0) {
        return 0;
    }

    int islands = 0;
    int rows = grid.length;
    int cols = grid[0].length;

    for (int r = 0; r < rows; r++) {
        for (int c = 0; c < cols; c++) {
            if (grid[r][c] == '1') {
                islands++;
                bfs(grid, r, c, rows, cols);
            }
        }
    }

    return islands;
}

private void bfs(char[][] grid, int r, int c, int rows, int cols) {
    Queue<int[]> q = new LinkedList<>();
    q.offer(new int[]{r, c});
    grid[r][c] = '0';

    int[][] directions = {{1, 0}, {-1, 0}, {0, 1}, {0, -1}};

    while (!q.isEmpty()) {
        int[] curr = q.poll();
        int row = curr[0];
        int col = curr[1];

        for (int[] dir : directions) {
            int nr = row + dir[0];
            int nc = col + dir[1];

            if (nr >= 0 && nr < rows && nc >= 0 && nc < cols && grid[nr][nc] == '1') {
                q.offer(new int[]{nr, nc});
                grid[nr][nc] = '0';
            }
        }
    }
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION


typedef struct {
    int r;
    int c;
} Point;

void bfs(char** grid, int r, int c, int rows, int cols) {
    // Simple queue implementation for BFS
    Point* queue = (Point*)malloc(rows * cols * sizeof(Point));
    int front = 0;
    int rear = 0;

    queue[rear++] = (Point){r, c};
    grid[r][c] = '0';

    int dr[] = {1, -1, 0, 0};
    int dc[] = {0, 0, 1, -1};

    while (front < rear) {
        Point curr = queue[front++];
        
        for (int i = 0; i < 4; i++) {
            int nr = curr.r + dr[i];
            int nc = curr.c + dc[i];

            if (nr >= 0 && nr < rows && nc >= 0 && nc < cols && grid[nr][nc] == '1') {
                queue[rear++] = (Point){nr, nc};
                grid[nr][nc] = '0';
            }
        }
    }
    free(queue);
}

int numIslands(char** grid, int gridSize, int* gridColSize) {
    if (gridSize == 0) return 0;
    int islands = 0;
    int rows = gridSize;
    int cols = gridColSize[0];

    for (int r = 0; r < rows; r++) {
        for (int c = 0; c < cols; c++) {
            if (grid[r][c] == '1') {
                islands++;
                bfs(grid, r, c, rows, cols);
            }
        }
    }
    return islands;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION


/**
 * @param {character[][]} grid
 * @return {number}
 */
var numIslands = function(grid) {
    if (!grid || grid.length === 0) return 0;

    let islands = 0;
    const rows = grid.length;
    const cols = grid[0].length;

    const bfs = (r, c) => {
        const queue = [];
        queue.push([r, c]);
        grid[r][c] = '0';

        const directions = [[1, 0], [-1, 0], [0, 1], [0, -1]];

        while (queue.length > 0) {
            const [currR, currC] = queue.shift();

            for (const [dr, dc] of directions) {
                const nr = currR + dr;
                const nc = currC + dc;

                if (nr >= 0 && nr < rows && nc >= 0 && nc < cols && grid[nr][nc] === '1') {
                    queue.push([nr, nc]);
                    grid[nr][nc] = '0';
                }
            }
        }
    };

    for (let r = 0; r < rows; r++) {
        for (let c = 0; c < cols; c++) {
            if (grid[r][c] === '1') {
                islands++;
                bfs(r, c);
            }
        }
    }

    return islands;
};

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def numIslands(grid: List[List[str]]) -> int:
    if not grid:
        return 0

    islands = 0
    rows, cols = len(grid), len(grid[0])

    for r in range(rows):
        for c in range(cols):
            if grid[r][c] == "1":
                islands += 1
                # Start BFS
                q = collections.deque()
                q.append((r, c))
                grid[r][c] = "0"

                while q:
                    row, col = q.popleft()
                    directions = [[1,0],[-1,0],[0,1],[0,-1]]

                    for dr, dc in directions:
                        nr, nc = row + dr, col + dc
                        if 0 <= nr < rows and 0 <= nc < cols and grid[nr][nc] == "1":
                            q.append((nr, nc))
                            grid[nr][nc] = "0"

    return islands

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  