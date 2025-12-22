## CPP

### SOLUTION

long long solve(int n, vector<long long> x) {
    const long long INF = 1e18;
    vector<long long> pre(n + 1, 0);
    for (int i = 0; i < n; i++) {
        pre[i + 1] = pre[i] + x[i];
    }

    vector<vector<pair<long long, int>>> dp(n + 2, vector<pair<long long, int>>(n + 2));

    for (int i = 1; i < n; i++) {
        dp[i][i + 1] = {pre[i + 1] - pre[i - 1], i};
    }

    for (int k = 3; k <= n; k++) {
        for (int i = 1; i + k - 1 <= n; i++) {
            int j = i + k - 1;
            int optLeft = dp[i][j - 1].second;
            int optRight = dp[i + 1][j].second;

            dp[i][j] = {INF, -1};
            long long currentSum = pre[j] - pre[i - 1];

            for (int split = optLeft; split <= optRight; split++) {
                long long val = dp[i][split].first + dp[split + 1][j].first;
                if (val < dp[i][j].first) {
                    dp[i][j] = {val, split};
                }
            }
            dp[i][j].first += currentSum;
        }
    }
    return dp[1][n].first;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static long solve(int n, long[] x) {
    long INF = 1L << 60;
    long[] pre = new long[n + 1];
    for (int i = 0; i < n; i++) {
        pre[i + 1] = pre[i] + x[i];
    }

    long[][] dpCost = new long[n + 2][n + 2];
    int[][] dpOpt = new int[n + 2][n + 2];

    for (int i = 1; i < n; i++) {
        dpCost[i][i + 1] = pre[i + 1] - pre[i - 1];
        dpOpt[i][i + 1] = i;
    }

    for (int k = 3; k <= n; k++) {
        for (int i = 1; i + k - 1 <= n; i++) {
            int j = i + k - 1;
            int optLeft = dpOpt[i][j - 1];
            int optRight = dpOpt[i + 1][j];
            
            dpCost[i][j] = INF;
            long currentSum = pre[j] - pre[i - 1];

            for (int split = optLeft; split <= optRight; split++) {
                long val = dpCost[i][split] + dpCost[split + 1][j];
                if (val < dpCost[i][j]) {
                    dpCost[i][j] = val;
                    dpOpt[i][j] = split;
                }
            }
            dpCost[i][j] += currentSum;
        }
    }
    return dpCost[1][n];
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  

