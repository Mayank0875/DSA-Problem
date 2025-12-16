## CPP

### SOLUTION

long long solve(int n, vector<int>& p) {
    long long totalSeats = 0;
    for (int seats : p) {
        totalSeats += seats;
    }

    // Sort descending
    sort(p.begin(), p.end(), greater<int>());

    long long threshold = totalSeats / 2;

    vector<long long> dp(totalSeats + 1, 0);
    dp[0] = 1;

    long long validCoalitions = 0;

    for (int x : p) {

        long long start = max(0LL, threshold - x + 1);

        for (long long s = start; s <= threshold; s++) {
            validCoalitions += dp[s];
        }

        // Update DP
        for (long long s = totalSeats; s >= x; s--) {
            dp[s] += dp[s - x];
        }
    }

    return validCoalitions;
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static long solve(int n, Integer[] p) {
    long totalSeats = 0;
    for (int seats : p) {
        totalSeats += seats;
    }

    // Sort descending
    Arrays.sort(p, Collections.reverseOrder());

    long threshold = totalSeats / 2;
    long[] dp = new long[(int)totalSeats + 1];
    dp[0] = 1;

    long validCoalitions = 0;

    for (int x : p) {
        
        long start = Math.max(0, threshold - x + 1);
        
        for (int s = (int)start; s <= threshold; s++) {
            validCoalitions += dp[s];
        }

        // Update DP
        for (int s = (int)totalSeats; s >= x; s--) {
            dp[s] += dp[s - x];
        }
    }

    return validCoalitions;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


