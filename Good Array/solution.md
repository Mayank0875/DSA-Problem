## CPP

### SOLUTION

long long GoodSubarray(vector<int> &arr){
    int n = arr.size();

    map<int, int> freq;
    freq[1]++;

    long long res = 0, cur = 0;
    for(int i = 0; i < n; ++i){
        cur += arr[i];
        res += freq[cur - i];
        freq[cur - i]++;
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

public static long GoodSubarray(int[] arr) {
    int n = arr.length;
    Map<Integer, Integer> freq = new HashMap<>();
    freq.put(1, 1);  

    long res = 0;
    int cur = 0;

    for (int i = 0; i < n; i++) {
        cur += arr[i];
        res += freq.getOrDefault(cur - i, 0);
        freq.put(cur - i, freq.getOrDefault(cur - i, 0) + 1);
    }

    return res;
}


### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## C

### SOLUTION

long long GoodSubarray(int* arr, int n) {
    long long res = 0;
    int cur = 0;
    int shift = n * 10;
    int size = 2 * shift + 5;

    long long* freq = (long long*)calloc(size, sizeof(long long));
    freq[shift + 1] = 1;  

    for (int i = 0; i < n; i++) {
        cur += arr[i];
        int key = cur - i + shift;
        res += freq[key];
        freq[key]++;
    }

    free(freq);
    return res;
}

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## JAVASCRIPT

### SOLUTION

function GoodSubarray(arr) {
    const n = arr.length;
    const freq = new Map();
    freq.set(1, 1);  

    let res = 0, cur = 0;
    for (let i = 0; i < n; i++) {
        cur += arr[i];
        const key = cur - i;
        res += freq.get(key) || 0;
        freq.set(key, (freq.get(key) || 0) + 1);
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



def GoodSubarray(arr: List[int]) -> int:
    freq = {1: 1} 

    res = 0
    cur = 0
    for i, val in enumerate(arr):
        cur += val
        key = cur - i
        res += freq.get(key, 0)
        freq[key] = freq.get(key, 0) + 1

    return res

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256
