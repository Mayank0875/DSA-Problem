## CPP

### SOLUTION

int ZeroOneQuery(vector<int>& arr, vector<vector<int>>& queries) {
    int n = arr.size();

    vector<int> prefix(n + 1, 0);
    for(int i = 1; i <= n; ++i){
        prefix[i] = prefix[i - 1] + arr[i - 1];
    }

    int result = 0;
    for(auto &q : queries){
        int one = prefix[q[1]] - prefix[q[0] - 1];
        int zero = q[1] - q[0] + 1 - one;

        result ^= ((q[2] == 1) ? one : zero);
    }

    return result;
}


### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## JAVA

### SOLUTION

public class Solution {
    public static int ZeroOneQuery(int[] arr, int[][] queries) {
        int n = arr.length;
        int[] prefix = new int[n + 1];

        for (int i = 0; i < n; i++) {
            prefix[i + 1] = prefix[i] + arr[i];
        }

        int result = 0;

        for (int[] q : queries) {
            int l = q[0], r = q[1], val = q[2];
            int ones = prefix[r] - prefix[l - 1];
            int zeros = (r - l + 1) - ones;

            result ^= (val == 1 ? ones : zeros);
        }

        return result;
    }
}


### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## C

### SOLUTION

int ZeroOneQuery(int* arr, int n, int queries[][3], int q) {
    int* prefix = (int*)calloc(n + 1, sizeof(int));
    for (int i = 0; i < n; i++) {
        prefix[i + 1] = prefix[i] + arr[i];
    }

    int result = 0;

    for (int i = 0; i < q; i++) {
        int l = queries[i][0];
        int r = queries[i][1];
        int val = queries[i][2];

        int ones = prefix[r] - prefix[l - 1];
        int zeros = (r - l + 1) - ones;

        result ^= (val == 1 ? ones : zeros);
    }

    free(prefix);
    return result;
}

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## JAVASCRIPT

### SOLUTION

function ZeroOneQuery(arr, queries) {
    const n = arr.length;
    const prefix = new Array(n + 1).fill(0);

    for (let i = 0; i < n; i++) {
        prefix[i + 1] = prefix[i] + arr[i];
    }

    let result = 0;

    for (let q of queries) {
        let l = q[0], r = q[1], val = q[2];
        let ones = prefix[r] - prefix[l - 1];
        let zeros = (r - l + 1) - ones;

        result ^= (val === 1 ? ones : zeros);
    }

    return result;
}


### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## PYTHON

### SOLUTION

def ZeroOneQuery(arr, queries):
    n = len(arr)
    prefix = [0] * (n + 1)

    for i in range(n):
        prefix[i + 1] = prefix[i] + arr[i]

    result = 0

    for q in queries:
        l, r, val = q
        ones = prefix[r] - prefix[l - 1]
        zeros = (r - l + 1) - ones
        result ^= ones if val == 1 else zeros

    return result

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256
