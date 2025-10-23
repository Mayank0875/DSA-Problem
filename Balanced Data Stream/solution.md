## CPP

### SOLUTION

int findShortestBalancingSegment(vector<int>& stream) {
    int n = stream.size();
    int ones = 0, zeros = 0;
    for(auto bit : stream){
        if(bit == 0) zeros++;
        else ones++;
    }

    int diff = ones - zeros;
    if(diff == 0){
        return 0;
    }
    map<int, int> freq;
    freq[0] = -1;

    int res = n;
    int curr = 0;
    for(int i = 0; i < n; ++i){
        curr += (stream[i] == 1 ? 1 : -1);

        int fin = curr - diff;
        if(freq.count(fin)){
            res = min(res, i - freq[fin]);
        }

        freq[curr] = i;
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

public static int findShortestBalancingSegment(int[] stream) {
    int n = stream.length;
    int ones = 0, zeros = 0;
    for (int bit : stream) {
        if (bit == 0) zeros++;
        else ones++;
    }

    int diff = ones - zeros;
    if (diff == 0) return 0;

    Map<Integer, Integer> freq = new HashMap<>();
    freq.put(0, -1);

    int res = n;
    int curr = 0;

    for (int i = 0; i < n; i++) {
        curr += (stream[i] == 1 ? 1 : -1);
        int fin = curr - diff;
        if (freq.containsKey(fin)) {
            res = Math.min(res, i - freq.get(fin));
        }
        freq.put(curr, i);
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

int findShortestBalancingSegment(int* stream, int n) {
    int ones = 0, zeros = 0;
    for (int i = 0; i < n; i++) {
        if (stream[i] == 0) zeros++;
        else ones++;
    }

    int diff = ones - zeros;
    if (diff == 0)
        return 0;

    int size = 4 * n + 10;      // large enough for shifts
    int *freq = (int*)malloc(size * sizeof(int));
    for (int i = 0; i < size; i++) freq[i] = INT_MIN;  // store index; -inf = not seen yet

    int shift = 2 * n;          // to avoid negative indices
    freq[shift + 0] = -1;       // freq[0] = -1

    int res = n;
    int curr = 0;

    for (int i = 0; i < n; i++) {
        curr += (stream[i] == 1 ? 1 : -1);

        int fin = curr - diff;

        // check if previously seen prefix = fin
        if (freq[shift + fin] != INT_MIN) {
            int len = i - freq[shift + fin];
            if (len < res) res = len;
        }

        // store first occurrence of curr
        if (freq[shift + curr] == INT_MIN)
            freq[shift + curr] = i;
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

function findShortestBalancingSegment(stream) {
    const n = stream.length;
    let ones = 0, zeros = 0;

    for (let bit of stream) {
        if (bit === 0) zeros++;
        else ones++;
    }

    const diff = ones - zeros;
    if (diff === 0) return 0;

    let freq = new Map();
    freq.set(0, -1);

    let res = n;
    let curr = 0;

    for (let i = 0; i < n; i++) {
        curr += (stream[i] === 1 ? 1 : -1);
        const fin = curr - diff;

        if (freq.has(fin)) {
            res = Math.min(res, i - freq.get(fin));
        }

        freq.set(curr, i);
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


def findShortestBalancingSegment(stream):
    n = len(stream)
    ones = stream.count(1)
    zeros = n - ones

    diff = ones - zeros
    if diff == 0:
        return 0

    freq = {0: -1}
    res = n
    curr = 0

    for i, bit in enumerate(stream):
        curr += 1 if bit == 1 else -1
        fin = curr - diff

        if fin in freq:
            res = min(res, i - freq[fin])

        freq[curr] = i

    return res

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256
