## CPP

### SOLUTION

class DisjointSets {
    vector<int> parents;
    vector<int> sizes;
public:
    DisjointSets(int n) : parents(n + 1), sizes(n + 1, 1) {
        iota(parents.begin(), parents.end(), 0);
    }
    int find(int x) {
        if (x == parents[x]) return x;
        return parents[x] = find(parents[x]);
    }
    void unite(int x, int y) {
        int rootX = find(x);
        int rootY = find(y);
        if (rootX != rootY) {
            if (sizes[rootX] < sizes[rootY]) swap(rootX, rootY);
            parents[rootY] = rootX;
            sizes[rootX] += sizes[rootY];
        }
    }
    int getSize(int x) {
        return sizes[find(x)];
    }
};

bool isProphetic(int n) {
    string s = to_string(n);
    for (char c : s) {
        if (c != '4' && c != '7') return false;
    }
    return true;
}

int minLinks(int n, vector<vector<int>>& edges) {
    DisjointSets dsu(n);
    for (const auto& edge : edges) {
        dsu.unite(edge[0], edge[1]);
    }

    map<int, int> componentCounts;
    vector<bool> visited(n + 1, false);
    
    for (int i = 1; i <= n; ++i) {
        int root = dsu.find(i);
        if (!visited[root]) {
            componentCounts[dsu.getSize(root)]++;
            visited[root] = true;
        }
    }

    const int INF = 1e9;
    vector<int> dp(n + 1, INF);
    dp[0] = 0;

    for (auto const& [weight, count] : componentCounts) {
        for (int r = 0; r < weight; ++r) {
            deque<pair<int, int>> dq; 
            for (int k = 0; k * weight + r <= n; ++k) {
                int currentWeight = k * weight + r;
                int val = dp[currentWeight] - k; 
                
                while (!dq.empty() && dq.back().first >= val) {
                    dq.pop_back();
                }
                dq.push_back({val, k});

                if (dq.front().second < k - count) {
                    dq.pop_front();
                }

                int bestVal = dq.front().first;
                if (bestVal > INF / 2) {
                } else {
                    dp[currentWeight] = min(dp[currentWeight], bestVal + k);
                }
            }
        }
    }

    int minRoads = INF;
    for (int i = 1; i <= n; ++i) {
        if (isProphetic(i) && dp[i] != INF) {
            minRoads = min(minRoads, dp[i] - 1);
        }
    }

    return (minRoads == INF) ? -1 : minRoads;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION


class DisjointSets {
    private int[] parents;
    private int[] sizes;

    public DisjointSets(int n) {
        parents = new int[n + 1];
        sizes = new int[n + 1];
        for (int i = 0; i <= n; i++) {
            parents[i] = i;
            sizes[i] = 1;
        }
    }

    public int find(int x) {
        if (x == parents[x]) return x;
        return parents[x] = find(parents[x]);
    }

    public void unite(int x, int y) {
        int rootX = find(x);
        int rootY = find(y);
        if (rootX != rootY) {
            if (sizes[rootX] < sizes[rootY]) {
                int temp = rootX; rootX = rootY; rootY = temp;
            }
            parents[rootY] = rootX;
            sizes[rootX] += sizes[rootY];
        }
    }

    public int getSize(int x) {
        return sizes[find(x)];
    }
}
    
private static boolean isProphetic(int n) {
    String s = String.valueOf(n);
    for (char c : s.toCharArray()) {
        if (c != '4' && c != '7') return false;
    }
    return true;
}

public static int minLinks(int n, int[][] edges) {
    DisjointSets dsu = new DisjointSets(n);
    for (int[] edge : edges) {
        dsu.unite(edge[0], edge[1]);
    }

    Map<Integer, Integer> componentCounts = new HashMap<>();
    boolean[] visited = new boolean[n + 1];

    for (int i = 1; i <= n; ++i) {
        int root = dsu.find(i);
        if (!visited[root]) {
            int size = dsu.getSize(root);
            componentCounts.put(size, componentCounts.getOrDefault(size, 0) + 1);
            visited[root] = true;
        }
    }

    final int INF = 1000000000;
    int[] dp = new int[n + 1];
    Arrays.fill(dp, INF);
    dp[0] = 0;

    for (Map.Entry<Integer, Integer> entry : componentCounts.entrySet()) {
        int weight = entry.getKey();
        int count = entry.getValue();

        for (int r = 0; r < weight; ++r) {
            Deque<int[]> dq = new ArrayDeque<>(); // {value, index}

            for (int k = 0; k * weight + r <= n; ++k) {
                int currentWeight = k * weight + r;
                int val = dp[currentWeight] - k;

                while (!dq.isEmpty() && dq.peekLast()[0] >= val) {
                    dq.pollLast();
                }
                dq.addLast(new int[]{val, k});

                if (dq.peekFirst()[1] < k - count) {
                    dq.pollFirst();
                }

                int bestVal = dq.peekFirst()[0];
                if (bestVal <= INF / 2) {
                    dp[currentWeight] = Math.min(dp[currentWeight], bestVal + k);
                }
            }
        }
    }

    int minRoads = INF;
    for (int i = 1; i <= n; ++i) {
        if (isProphetic(i) && dp[i] != INF) {
            minRoads = Math.min(minRoads, dp[i] - 1);
        }
    }

    return (minRoads == INF) ? -1 : minRoads;
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  

