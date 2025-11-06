## CPP

### SOLUTION

bool exist(vector<vector<char>>& board, string word) {
    int rows = board.size();
    int cols = board[0].size();
    unordered_set<string> visited;

    auto dfs = [&](int r, int c, int k, auto& dfs) -> bool {
        if (k == word.length()) {
            return true;
        }

        if (r < 0 || r >= rows || c < 0 || c >= cols || visited.count(to_string(r) + "," + to_string(c)) || board[r][c] != word[k]) {
            return false;
        }

        visited.insert(to_string(r) + "," + to_string(c));
        bool res = dfs(r + 1, c, k + 1, dfs) || dfs(r - 1, c, k + 1, dfs) || dfs(r, c + 1, k + 1, dfs) || dfs(r, c - 1, k + 1, dfs);
        visited.erase(to_string(r) + "," + to_string(c));
        return res;
    };

    unordered_map<char, int> count;
    for (char c : word) {
        count[c]++;
    }

    if (count[word[0]] > count[word.back()]) {
        reverse(word.begin(), word.end());
    }

    for (int r = 0; r < rows; r++) {
        for (int c = 0; c < cols; c++) {
            if (dfs(r, c, 0, dfs)) {
                return true;
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

static int rows, cols;
static char[][] board;
static String word;
static Set<String> visited;

static boolean dfs(int r, int c, int k) {
    if (k == word.length()) return true;
    if (r < 0 || r >= rows || c < 0 || c >= cols ||
        visited.contains(r + "," + c) || board[r][c] != word.charAt(k))
        return false;

    visited.add(r + "," + c);
    boolean res = dfs(r + 1, c, k + 1) ||
                    dfs(r - 1, c, k + 1) ||
                    dfs(r, c + 1, k + 1) ||
                    dfs(r, c - 1, k + 1);
    visited.remove(r + "," + c);
    return res;
}

public static boolean exist(char[][] b, String w) {
    board = b;
    word = w;
    rows = board.length;
    cols = board[0].length;
    visited = new HashSet<>();

    // small optimization: reverse if starting char rarer
    Map<Character, Integer> count = new HashMap<>();
    for (char ch : word.toCharArray()) count.put(ch, count.getOrDefault(ch, 0) + 1);
    if (count.getOrDefault(word.charAt(0), 0) > count.getOrDefault(word.charAt(word.length() - 1), 0))
        word = new StringBuilder(word).reverse().toString();

    for (int r = 0; r < rows; r++) {
        for (int c = 0; c < cols; c++) {
            if (dfs(r, c, 0)) return true;
        }
    }
    return false;
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

bool dfs(char** board, int rows, int cols, int r, int c, char* word, int len, int k, bool** visited) {
    if (k == len) return true;
    if (r < 0 || r >= rows || c < 0 || c >= cols || visited[r][c] || board[r][c] != word[k]) return false;

    visited[r][c] = true;
    bool res = dfs(board, rows, cols, r + 1, c, word, len, k + 1, visited) ||
               dfs(board, rows, cols, r - 1, c, word, len, k + 1, visited) ||
               dfs(board, rows, cols, r, c + 1, word, len, k + 1, visited) ||
               dfs(board, rows, cols, r, c - 1, word, len, k + 1, visited);
    visited[r][c] = false;
    return res;
}

bool exist(char** board, int boardSize, int* boardColSize, char* word) {
    int rows = boardSize, cols = boardColSize[0], len = strlen(word);

    int count[256] = {0};
    for (int i = 0; i < len; i++) count[(unsigned char)word[i]]++;
    if (count[(unsigned char)word[0]] > count[(unsigned char)word[len - 1]]) {
        for (int i = 0; i < len / 2; i++) {
            char tmp = word[i];
            word[i] = word[len - 1 - i];
            word[len - 1 - i] = tmp;
        }
    }

    bool** visited = malloc(rows * sizeof(bool*));
    for (int i = 0; i < rows; i++) {
        visited[i] = calloc(cols, sizeof(bool));
    }

    for (int r = 0; r < rows; r++) {
        for (int c = 0; c < cols; c++) {
            if (dfs(board, rows, cols, r, c, word, len, 0, visited)) {
                for (int i = 0; i < rows; i++) free(visited[i]);
                free(visited);
                return true;
            }
        }
    }

    for (int i = 0; i < rows; i++) free(visited[i]);
    free(visited);
    return false;
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function exist(board, word) {
    const rows = board.length;
    const cols = board[0].length;
    const visited = new Set();

    function dfs(r, c, k) {
        if (k === word.length) return true;
        if (r < 0 || r >= rows || c < 0 || c >= cols ||
            visited.has(`${r},${c}`) || board[r][c] !== word[k]) return false;

        visited.add(`${r},${c}`);
        const res = dfs(r + 1, c, k + 1) ||
                    dfs(r - 1, c, k + 1) ||
                    dfs(r, c + 1, k + 1) ||
                    dfs(r, c - 1, k + 1);
        visited.delete(`${r},${c}`);
        return res;
    }

    const count = {};
    for (const ch of word) count[ch] = (count[ch] || 0) + 1;
    if (count[word[0]] > count[word[word.length - 1]]) {
        word = word.split('').reverse().join('');
    }

    for (let r = 0; r < rows; r++) {
        for (let c = 0; c < cols; c++) {
            if (dfs(r, c, 0)) return true;
        }
    }
    return false;
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def exist(board, word):
    rows, cols = len(board), len(board[0])
    visited = set()

    def dfs(r, c, k):
        if k == len(word):
            return True
        if r < 0 or r >= rows or c < 0 or c >= cols or (r, c) in visited or board[r][c] != word[k]:
            return False

        visited.add((r, c))
        res = (dfs(r + 1, c, k + 1) or
               dfs(r - 1, c, k + 1) or
               dfs(r, c + 1, k + 1) or
               dfs(r, c - 1, k + 1))
        visited.remove((r, c))
        return res

    count = {}
    for ch in word:
        count[ch] = count.get(ch, 0) + 1

    if count[word[0]] > count[word[-1]]:
        word = word[::-1]

    for r in range(rows):
        for c in range(cols):
            if dfs(r, c, 0):
                return True
    return False

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  