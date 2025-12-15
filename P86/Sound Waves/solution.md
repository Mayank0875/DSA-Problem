## CPP

### SOLUTION

bool canEscape(int n, int m, vector<string>& maze) {
    const int INF = 1000000000;
    queue<pair<int,int>> q_monsters;
    vector<vector<int>> dist_monsters(n, vector<int>(m, INF));
    int start_r = -1, start_c = -1;

    for (int i = 0; i < n; ++i) {
        for (int j = 0; j < m; ++j) {
            if (maze[i][j] == 'M') {
                q_monsters.push({i, j});
                dist_monsters[i][j] = 0;
            } else if (maze[i][j] == 'A') {
                start_r = i;
                start_c = j;
            }
        }
    }

    if (start_r == -1) return false;

    int dr[] = {-1, 1, 0, 0};
    int dc[] = {0, 0, -1, 1};

    while (!q_monsters.empty()) {
        auto [r, c] = q_monsters.front();
        q_monsters.pop();
        for (int k = 0; k < 4; ++k) {
            int nr = r + dr[k];
            int nc = c + dc[k];
            if (nr >= 0 && nr < n && nc >= 0 && nc < m && maze[nr][nc] != '#' && dist_monsters[nr][nc] == INF) {
                dist_monsters[nr][nc] = dist_monsters[r][c] + 1;
                q_monsters.push({nr, nc});
            }
        }
    }

    if (start_r == 0 || start_r == n - 1 || start_c == 0 || start_c == m - 1) {
        if (0 < dist_monsters[start_r][start_c]) return true;
    }

    queue<pair<int,int>> q_player;
    vector<vector<int>> dist_player(n, vector<int>(m, -1));
    q_player.push({start_r, start_c});
    dist_player[start_r][start_c] = 0;

    while (!q_player.empty()) {
        auto [r, c] = q_player.front();
        q_player.pop();
        for (int k = 0; k < 4; ++k) {
            int nr = r + dr[k];
            int nc = c + dc[k];
            if (nr >= 0 && nr < n && nc >= 0 && nc < m && maze[nr][nc] != '#' && dist_player[nr][nc] == -1) {
                if (dist_player[r][c] + 1 < dist_monsters[nr][nc]) {
                    dist_player[nr][nc] = dist_player[r][c] + 1;
                    if (nr == 0 || nr == n - 1 || nc == 0 || nc == m - 1) return true;
                    q_player.push({nr, nc});
                }
            }
        }
    }
    return false;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static boolean canEscape(int n, int m, char[][] maze) {
    int INF = 1000000000;
    int[][] distMon = new int[n][m];
    for (int[] row : distMon) Arrays.fill(row, INF);

    Queue<int[]> qMon = new ArrayDeque<>();
    int startR = -1, startC = -1;

    for (int i = 0; i < n; i++) {
        for (int j = 0; j < m; j++) {
            if (maze[i][j] == 'M') {
                qMon.add(new int[]{i, j});
                distMon[i][j] = 0;
            } else if (maze[i][j] == 'A') {
                startR = i;
                startC = j;
            }
        }
    }

    if (startR == -1) return false;

    int[] dr = {-1, 1, 0, 0};
    int[] dc = {0, 0, -1, 1};

    while (!qMon.isEmpty()) {
        int[] cur = qMon.poll();
        int r = cur[0], c = cur[1];
        for (int k = 0; k < 4; k++) {
            int nr = r + dr[k];
            int nc = c + dc[k];
            if (nr >= 0 && nr < n && nc >= 0 && nc < m && maze[nr][nc] != '#' && distMon[nr][nc] == INF) {
                distMon[nr][nc] = distMon[r][c] + 1;
                qMon.add(new int[]{nr, nc});
            }
        }
    }

    if (startR == 0 || startR == n - 1 || startC == 0 || startC == m - 1) {
        if (0 < distMon[startR][startC]) return true;
    }

    int[][] distP = new int[n][m];
    for (int[] row : distP) Arrays.fill(row, -1);

    Queue<int[]> qP = new ArrayDeque<>();
    qP.add(new int[]{startR, startC});
    distP[startR][startC] = 0;

    while (!qP.isEmpty()) {
        int[] cur = qP.poll();
        int r = cur[0], c = cur[1];
        for (int k = 0; k < 4; k++) {
            int nr = r + dr[k], nc = c + dc[k];
            if (nr >= 0 && nr < n && nc >= 0 && nc < m && maze[nr][nc] != '#' && distP[nr][nc] == -1) {
                if (distP[r][c] + 1 < distMon[nr][nc]) {
                    distP[nr][nc] = distP[r][c] + 1;
                    if (nr == 0 || nr == n - 1 || nc == 0 || nc == m - 1) return true;
                    qP.add(new int[]{nr, nc});
                }
            }
        }
    }

    return false;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


