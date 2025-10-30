## CPP

### SOLUTION

int gcd(int a, int b) {
    if (b == 0) return a;
    return gcd(b, a % b);
}

int MaximumGCD(vector<int> & arr){
    int n = arr.size();
    vector<int> prefix(n + 1, 0), suffix(n + 2, 0);

    for(int i = 0; i < n; ++i){
        prefix[i + 1] = gcd(prefix[i], arr[i]);
    }

    for(int i = n - 1; i >= 0; --i){
        suffix[i + 1] = gcd(suffix[i + 2], arr[i]);
    }

    int res = 1;

    for(int i = 1; i <= n; ++i){
        res = max(res, gcd(prefix[i - 1], suffix[i + 1]));
    }

    return res;
}


### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## JAVA

### SOLUTION

public static int MaximumGCD(int[] arr) {
    int n = arr.length;
    int[] prefix = new int[n + 1];
    int[] suffix = new int[n + 2];

    for (int i = 0; i < n; i++) {
        prefix[i + 1] = gcd(prefix[i], arr[i]);
    }

    for (int i = n - 1; i >= 0; i--) {
        suffix[i + 1] = gcd(suffix[i + 2], arr[i]);
    }

    int res = 1;
    for (int i = 1; i <= n; i++) {
        res = Math.max(res, gcd(prefix[i - 1], suffix[i + 1]));
    }

    return res;
}

private static int gcd(int a, int b) {
    if (b == 0) return a;
    return gcd(b, a % b);
}



### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## C

### SOLUTION

int gcd(int a, int b) {
    return b == 0 ? a : gcd(b, a % b);
}

int MaximumGCD(int arr[], int n) {
    int* prefix = (int*)calloc(n + 1, sizeof(int));
    int* suffix = (int*)calloc(n + 2, sizeof(int));

    for (int i = 0; i < n; i++) {
        prefix[i + 1] = gcd(prefix[i], arr[i]);
    }

    for (int i = n - 1; i >= 0; i--) {
        suffix[i + 1] = gcd(suffix[i + 2], arr[i]);
    }

    int res = 1;
    for (int i = 1; i <= n; i++) {
        int g = gcd(prefix[i - 1], suffix[i + 1]);
        if (g > res) res = g;
    }

    free(prefix);
    free(suffix);
    return res;
}

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## JAVASCRIPT

### SOLUTION

function gcd(a, b) {
    return b === 0 ? a : gcd(b, a % b);
}

function MaximumGCD(arr) {
    const n = arr.length;
    const prefix = new Array(n + 1).fill(0);
    const suffix = new Array(n + 2).fill(0);

    for (let i = 0; i < n; i++) {
        prefix[i + 1] = gcd(prefix[i], arr[i]);
    }

    for (let i = n - 1; i >= 0; i--) {
        suffix[i + 1] = gcd(suffix[i + 2], arr[i]);
    }

    let res = 1;
    for (let i = 1; i <= n; i++) {
        res = Math.max(res, gcd(prefix[i - 1], suffix[i + 1]));
    }

    return res;
}


### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## PYTHON

### SOLUTION

def gcd(a, b):
    if b == 0:
        return a
    return gcd(b, a % b)

def MaximumGCD(arr: List[int]) -> int:
    n = len(arr)
    prefix = [0] * (n + 1)
    suffix = [0] * (n + 2)

    for i in range(n):
        prefix[i + 1] = gcd(prefix[i], arr[i])

    for i in range(n - 1, -1, -1):
        suffix[i + 1] = gcd(suffix[i + 2], arr[i])

    res = 1
    for i in range(1, n + 1):
        res = max(res, gcd(prefix[i - 1], suffix[i + 1]))

    return res


### METADATA

**TimeLimit**
2000

**MemoryLimit**
256
