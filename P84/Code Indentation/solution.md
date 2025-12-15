## CPP

### SOLUTION


vector<vector<long long>> multiply(const vector<vector<long long>>& A,
                                   const vector<vector<long long>>& B) {
    int MOD = 1000000007;

    vector<vector<long long>> C(6, vector<long long>(6, 0));
    for (int i = 0; i < 6; i++) {
        for (int k = 0; k < 6; k++) {
            if (A[i][k] == 0) continue;
            for (int j = 0; j < 6; j++) {
                C[i][j] = (C[i][j] + A[i][k] * B[k][j]) % MOD;
            }
        }
    }
    return C;
}

vector<vector<long long>> power(vector<vector<long long>> A, long long p) {
    vector<vector<long long>> res(6, vector<long long>(6, 0));
    for (int i = 0; i < 6; i++) res[i][i] = 1;

    while (p > 0) {
        if (p & 1) res = multiply(res, A);
        A = multiply(A, A);
        p >>= 1;
    }
    return res;
}

int countWays(long long n) {
    vector<vector<long long>> T(6, vector<long long>(6, 0));

    for (int i = 0; i < 5; i++) {
        T[i][i + 1] = 1;
    }
    for (int i = 0; i < 6; i++) {
        T[5][i] = 1;
    }

    vector<vector<long long>> result = power(T, n);
    return result[5][5];
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

private static long[][] multiply(long[][] A, long[][] B) {
    int MOD = 1000000007;

    long[][] C = new long[6][6];
    for (int i = 0; i < 6; i++) {
        for (int k = 0; k < 6; k++) {
            if (A[i][k] == 0) continue;
            for (int j = 0; j < 6; j++) {
                C[i][j] = (C[i][j] + A[i][k] * B[k][j]) % MOD;
            }
        }
    }
    return C;
}

private static long[][] power(long[][] A, long p) {
    long[][] res = new long[6][6];
    for (int i = 0; i < 6; i++) res[i][i] = 1;

    while (p > 0) {
        if ((p & 1) == 1) res = multiply(res, A);
        A = multiply(A, A);
        p >>= 1;
    }
    return res;
}

public static int countWays(long n) {
    long[][] T = new long[6][6];

    for (int i = 0; i < 5; i++) {
        T[i][i + 1] = 1;
    }
    for (int i = 0; i < 6; i++) {
        T[5][i] = 1;
    }

    long[][] result = power(T, n);
    return (int) result[5][5];
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  

