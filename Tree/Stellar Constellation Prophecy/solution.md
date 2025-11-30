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

int minLinks(int n, const vector<vector<int>>& edges) {
    DisjointSets dsu(n);
    for (const auto& edge : edges) {
        dsu.unite(edge[0], edge[1]);
    }

    map<int, int> componentCounts; // size -> frequency
    vector<bool> visited(n + 1, false);
    
    for (int i = 1; i <= n; ++i) {
        int root = dsu.find(i);
        if (!visited[root]) {
            componentCounts[dsu.getSize(root)]++;
            visited[root] = true;
        }
    }

    // dp[i] = min components needed to get exactly size i
    const int INF = 1e9;
    vector<int> dp(n + 1, INF);
    dp[0] = 0;

    // Bounded Knapsack Optimization using Deque (Sliding Window Minimum)
    for (auto const& [weight, count] : componentCounts) {
        for (int r = 0; r < weight; ++r) {
            deque<pair<int, int>> dq; // {value, index}
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
                if (bestVal != INF - k && bestVal + k < dp[currentWeight]) { // Check bounds carefully with INF
                     // Actually easier: if original dp[idx] was INF, val is huge. 
                     // We just check if result is valid.
                     if (dq.front().first > INF / 2) { 
                         // Logic: INF - something small is still large. 
                         // Valid transition means dq.front().first comes from a reachable state.
                     } else {
                         dp[currentWeight] = min(dp[currentWeight], bestVal + k);
                     }
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


class DSU {
    int[] parent;
    int[] size;

    DSU(int n) {
        parent = new int[n + 1];
        size = new int[n + 1];
        for (int i = 0; i <= n; ++i) {
            parent[i] = i;
            size[i] = 1;
        }
    }

    int find(int x) {
        if (parent[x] == x) return x;
        return parent[x] = find(parent[x]);
    }

    void unite(int x, int y) {
        int rx = find(x), ry = find(y);
        if (rx == ry) return;
        if (size[rx] < size[ry]) {
            int t = rx; rx = ry; ry = t;
        }
        parent[ry] = rx;
        size[rx] += size[ry];
    }
}


static final int INF = 1_000_000_000;


public static int minLinks(int n, List<List<Integer>> edges) {
    int n = 1;
    for (List<Integer> e : edges) {
        if (e.size() >= 1) n = Math.max(n, e.get(0));
        if (e.size() >= 2) n = Math.max(n, e.get(1));
    }

    // Build DSU and unite edges
    DSU dsu = new DSU(n);
    for (List<Integer> e : edges) {
        if (e.size() >= 2) {
            int u = e.get(0);
            int v = e.get(1);
            dsu.unite(u, v);
        }
    }

    Map<Integer, Integer> counts = new HashMap<>();
    boolean[] seenRoot = new boolean[n + 1];
    for (int i = 1; i <= n; ++i) {
        int r = dsu.find(i);
        if (!seenRoot[r]) {
            int sz = dsu.size[r];
            counts.put(sz, counts.getOrDefault(sz, 0) + 1);
            seenRoot[r] = true;
        }
    }

    int[] dp = new int[n + 1];
    Arrays.fill(dp, INF);
    dp[0] = 0;

    for (Map.Entry<Integer, Integer> entry : counts.entrySet()) {
        int weight = entry.getKey();
        int count = entry.getValue();

        for (int r = 0; r < weight; ++r) {
            Deque<int[]> dq = new ArrayDeque<>(); // each element: {val, k}
            int maxK = (n - r) / weight;
            for (int k = 0; k <= maxK; ++k) {
                int idx = k * weight + r;
                int val = dp[idx] == INF ? INF : dp[idx] - k;

                // Maintain monotonic increasing deque by val
                while (!dq.isEmpty() && dq.peekLast()[0] >= val) dq.pollLast();
                dq.addLast(new int[]{val, k});

                // Remove elements out of window (k - count)
                while (!dq.isEmpty() && dq.peekFirst()[1] < k - count) dq.pollFirst();

                // Use best from front
                if (!dq.isEmpty()) {
                    int bestVal = dq.peekFirst()[0];
                    if (bestVal <= INF / 2) {
                        int candidate = bestVal + k;
                        if (candidate < dp[idx]) dp[idx] = candidate;
                    }
                }
            }
        }
    }

    int answer = INF;
    for (int i = 1; i <= n; ++i) {
        if (dp[i] != INF && isProphetic(i)) {
            answer = Math.min(answer, dp[i] - 1); // components used - 1 => edges to add
        }
    }
    return (answer == INF) ? -1 : answer;
}

private static boolean isProphetic(int x) {
    if (x <= 0) return false;
    while (x > 0) {
        int d = x % 10;
        if (d != 4 && d != 7) return false;
        x /= 10;
    }
    return true;
}

### METADATA

**TimeLimit**
1000

**MemoryLimit**
512



## C

### SOLUTION

#include <stdio.h>
#include <stdlib.h>
#include <stdbool.h>
#include <string.h>

#define INF 1000000000

typedef struct {
    int *parents;
    int *sizes;
} DSU;

void initDSU(DSU *dsu, int n) {
    dsu->parents = (int*)malloc((n + 1) * sizeof(int));
    dsu->sizes = (int*)malloc((n + 1) * sizeof(int));
    for (int i = 0; i <= n; i++) {
        dsu->parents[i] = i;
        dsu->sizes[i] = 1;
    }
}

int findDSU(DSU *dsu, int x) {
    if (dsu->parents[x] == x) return x;
    return dsu->parents[x] = findDSU(dsu, dsu->parents[x]);
}

void uniteDSU(DSU *dsu, int x, int y) {
    int rootX = findDSU(dsu, x);
    int rootY = findDSU(dsu, y);
    if (rootX != rootY) {
        if (dsu->sizes[rootX] < dsu->sizes[rootY]) {
            int temp = rootX; rootX = rootY; rootY = temp;
        }
        dsu->parents[rootY] = rootX;
        dsu->sizes[rootX] += dsu->sizes[rootY];
    }
}

bool isProphetic(int n) {
    while (n > 0) {
        int d = n % 10;
        if (d != 4 && d != 7) return false;
        n /= 10;
    }
    return true;
}

// Queue structure for Deque optimization
typedef struct {
    int val;
    int idx;
} Pair;

int minLinks(int n, int m, int** edges) {
    DSU dsu;
    initDSU(&dsu, n);
    for (int i = 0; i < m; i++) {
        uniteDSU(&dsu, edges[i][0], edges[i][1]);
    }

    int *counts = (int*)calloc(n + 1, sizeof(int));
    bool *visited = (bool*)calloc(n + 1, sizeof(bool));
    int *distinctWeights = (int*)malloc((n + 1) * sizeof(int));
    int distinctCount = 0;

    for (int i = 1; i <= n; i++) {
        int root = findDSU(&dsu, i);
        if (!visited[root]) {
            int sz = dsu.sizes[root];
            if (counts[sz] == 0) {
                distinctWeights[distinctCount++] = sz;
            }
            counts[sz]++;
            visited[root] = true;
        }
    }

    int *dp = (int*)malloc((n + 1) * sizeof(int));
    for(int i=0; i<=n; i++) dp[i] = INF;
    dp[0] = 0;

    // Deque buffer
    Pair *dq = (Pair*)malloc((n + 1) * sizeof(Pair));

    for (int i = 0; i < distinctCount; i++) {
        int weight = distinctWeights[i];
        int count = counts[weight];

        for (int r = 0; r < weight; r++) {
            int head = 0, tail = 0; // Deque pointers
            
            for (int k = 0; k * weight + r <= n; k++) {
                int currentWeight = k * weight + r;
                int val = dp[currentWeight] - k;

                while (head < tail && dq[tail - 1].val >= val) {
                    tail--;
                }
                dq[tail].val = val;
                dq[tail].idx = k;
                tail++;

                if (dq[head].idx < k - count) {
                    head++;
                }

                int bestVal = dq[head].val;
                if (bestVal <= INF / 2) {
                    if (bestVal + k < dp[currentWeight]) {
                        dp[currentWeight] = bestVal + k;
                    }
                }
            }
        }
    }

    int minRoads = INF;
    for (int i = 1; i <= n; i++) {
        if (isProphetic(i) && dp[i] != INF) {
            if (dp[i] - 1 < minRoads) minRoads = dp[i] - 1;
        }
    }

    free(dsu.parents); free(dsu.sizes);
    free(counts); free(visited); free(distinctWeights);
    free(dp); free(dq);

    return (minRoads == INF) ? -1 : minRoads;
}

### METADATA

**TimeLimit**
1000

**MemoryLimit**
512



## JAVASCRIPT

### SOLUTION

function minLinks(n, edges) {
    const parent = new Array(n + 1).fill(0).map((_, i) => i);
    const size = new Array(n + 1).fill(1);

    function find(x) {
        if (parent[x] === x) return x;
        return parent[x] = find(parent[x]);
    }

    function unite(x, y) {
        let rootX = find(x);
        let rootY = find(y);
        if (rootX !== rootY) {
            if (size[rootX] < size[rootY]) [rootX, rootY] = [rootY, rootX];
            parent[rootY] = rootX;
            size[rootX] += size[rootY];
        }
    }

    for (const [u, v] of edges) {
        unite(u, v);
    }

    const counts = new Map();
    const visited = new Array(n + 1).fill(false);

    for (let i = 1; i <= n; i++) {
        const root = find(i);
        if (!visited[root]) {
            const sz = size[root];
            counts.set(sz, (counts.get(sz) || 0) + 1);
            visited[root] = true;
        }
    }

    const INF = 1e9;
    const dp = new Array(n + 1).fill(INF);
    dp[0] = 0;

    for (const [weight, count] of counts) {
        for (let r = 0; r < weight; r++) {
            const dq = []; // Array of {val, idx}
            
            // Sliding window using array as deque
            // Optimization: Use a pointer index for head to avoid shift() O(N)
            let head = 0;
            
            for (let k = 0; k * weight + r <= n; k++) {
                const currentWeight = k * weight + r;
                const val = dp[currentWeight] - k;

                while (dq.length > head && dq[dq.length - 1].val >= val) {
                    dq.pop();
                }
                dq.push({ val, idx: k });

                if (dq[head].idx < k - count) {
                    head++;
                }

                const bestVal = dq[head].val;
                if (bestVal <= INF / 2) {
                    dp[currentWeight] = Math.min(dp[currentWeight], bestVal + k);
                }
            }
        }
    }

    function isProphetic(num) {
        const s = num.toString();
        for (let i = 0; i < s.length; i++) {
            if (s[i] !== '4' && s[i] !== '7') return false;
        }
        return true;
    }

    let minRoads = INF;
    for (let i = 1; i <= n; i++) {
        if (isProphetic(i) && dp[i] !== INF) {
            minRoads = Math.min(minRoads, dp[i] - 1);
        }
    }

    return (minRoads === INF) ? -1 : minRoads;
}

### METADATA

**TimeLimit**
1000

**MemoryLimit**
512



## PYTHON

### SOLUTION




def minLinks(n: int, edges: list) -> int:
    parent = list(range(n + 1))
    size = [1] * (n + 1)

    def find(x):
        if parent[x] != x:
            parent[x] = find(parent[x])
        return parent[x]

    def unite(x, y):
        rootX = find(x)
        rootY = find(y)
        if rootX != rootY:
            if size[rootX] < size[rootY]:
                rootX, rootY = rootY, rootX
            parent[rootY] = rootX
            size[rootX] += size[rootY]

    for u, v in edges:
        unite(u, v)

    counts = {}
    visited = [False] * (n + 1)

    for i in range(1, n + 1):
        root = find(i)
        if not visited[root]:
            sz = size[root]
            counts[sz] = counts.get(sz, 0) + 1
            visited[root] = True

    INF = 10**9
    dp = [INF] * (n + 1)
    dp[0] = 0

    # Bounded Knapsack with Deque Optimization
    # Sorting keys might slightly improve cache locality
    for weight, count in counts.items():
        for r in range(weight):
            dq = deque()
            
            # Iterate k such that currentWeight = k * weight + r <= n
            # max_k = (n - r) // weight
            for k in range((n - r) // weight + 1):
                current_weight = k * weight + r
                val = dp[current_weight] - k
                
                while dq and dq[-1][0] >= val:
                    dq.pop()
                dq.append((val, k))
                
                if dq[0][1] < k - count:
                    dq.popleft()
                
                best_val = dq[0][0]
                if best_val <= INF // 2:
                    if best_val + k < dp[current_weight]:
                        dp[current_weight] = best_val + k

    def is_prophetic(num):
        return all(c in '47' for c in str(num))

    min_roads = INF
    for i in range(1, n + 1):
        if dp[i] != INF and is_prophetic(i):
            min_roads = min(min_roads, dp[i] - 1)

    return -1 if min_roads == INF else min_roads

### METADATA

**TimeLimit**
1000

**MemoryLimit**
512