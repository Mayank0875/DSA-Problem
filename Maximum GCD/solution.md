## CPP

### SOLUTION

long long OrdinaryPairs(vector<int>& arr, int X) {
    int n = arr.size();

    long long result = 0;
    map<long long, long long> freq;

    for(int i = 0; i < n; ++i){
        int add = (X - arr[i] % X) % X;

        if((1LL * add * arr[i]) % X == 0){
            result += freq[add];
        }

        freq[arr[i] % X]++;
    }

    return result;
}

### METADATA

**TimeLimit**
1000

**MemoryLimit**
256

## JAVA

### SOLUTION

public static long OrdinaryPairs(int[] arr, int X) {
    int n = arr.length;
    long result = 0;
    Map<Integer, Long> freq = new HashMap<>();

    for(int i = 0; i < n; i++){
        int add = (X - arr[i] % X) % X;

        if((1L * add * arr[i]) % X == 0){
            result += freq.getOrDefault(add, 0L);
        }

        freq.put(arr[i] % X, freq.getOrDefault(arr[i] % X, 0L) + 1);
    }

    return result;
}


### METADATA

**TimeLimit**
1000

**MemoryLimit**
256

## C

### SOLUTION

long long OrdinaryPairs(int arr[], int n, int X) {
    long long result = 0;
    long long* freq = (long long*)calloc(X, sizeof(long long));

    for(int i = 0; i < n; i++){
        int add = (X - arr[i] % X) % X;

        if((1LL * add * arr[i]) % X == 0){
            result += freq[add];
        }

        freq[arr[i] % X]++;
    }

    free(freq);
    return result;
}

### METADATA

**TimeLimit**
1000

**MemoryLimit**
256

## JAVASCRIPT

### SOLUTION

function OrdinaryPairs(arr, X) {
    let result = 0;
    let freq = new Map();

    for(let i = 0; i < arr.length; i++){
        let add = (X - arr[i] % X) % X;

        if((add * arr[i]) % X === 0){
            result += freq.get(add) || 0;
        }

        freq.set(arr[i] % X, (freq.get(arr[i] % X) || 0) + 1);
    }

    return result;
}


### METADATA

**TimeLimit**
1000

**MemoryLimit**
256

## PYTHON

### SOLUTION

def OrdinaryPairs(arr, X):
    from collections import defaultdict
    result = 0
    freq = defaultdict(int)

    for num in arr:
        add = (X - num % X) % X

        if (add * num) % X == 0:
            result += freq[add]

        freq[num % X] += 1

    return result


### METADATA

**TimeLimit**
1000

**MemoryLimit**
256
