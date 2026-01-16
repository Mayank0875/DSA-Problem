## CPP

### SOLUTION

const int MAXN = 500005;
int spf[MAXN];
long long prefixCount[MAXN];

void precompute() {
    for (int i = 0; i < MAXN; i++) spf[i] = i;
    for (int i = 2; i * i < MAXN; i++) {
        if (spf[i] == i) {
            for (int j = i * i; j < MAXN; j += i)
                if (spf[j] == j) spf[j] = i;
        }
    }
    prefixCount[0] = 0;
    for (int i = 1; i < MAXN; i++) {
        int factors = 0;
        int temp = i;
        while (temp > 1) {
            temp /= spf[temp];
            factors++;
        }
        prefixCount[i] = prefixCount[i - 1] + factors;
    }
}

long long maxRounds(int a, int b) {
    if (spf[1] == 0) precompute(); // Ensure initialized
    return prefixCount[a] - prefixCount[b];
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

static final int MAXN = 500005;
static int[] spf = new int[MAXN];
static long[] prefixCount = new long[MAXN];
static boolean initialized = false;

public static void precompute() {
    if (initialized) return;
    for (int i = 0; i < MAXN; i++) spf[i] = i;
    for (int i = 2; i * i < MAXN; i++) {
        if (spf[i] == i) {
            for (int j = i * i; j < MAXN; j += i)
                if (spf[j] == j) spf[j] = i;
        }
    }
    for (int i = 2; i < MAXN; i++) {
        int factors = 0;
        int temp = i;
        while (temp > 1) {
            temp /= spf[temp];
            factors++;
        }
        prefixCount[i] = prefixCount[i - 1] + factors;
    }
    initialized = true;
}

public static long maxRounds(int a, int b) {
    if (!initialized) precompute();
    return prefixCount[a] - prefixCount[b];
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

#define MAXN 500005

int spf[MAXN];
long long prefixCount[MAXN];
int initialized = 0;

void precompute() {
    for (int i = 0; i < MAXN; i++) spf[i] = i;
    for (int i = 2; i * i < MAXN; i++) {
        if (spf[i] == i) {
            for (int j = i * i; j < MAXN; j += i)
                if (spf[j] == j) spf[j] = i;
        }
    }
    prefixCount[0] = 0;
    for (int i = 1; i < MAXN; i++) {
        int factors = 0;
        int temp = i;
        while (temp > 1) {
            temp /= spf[temp];
            factors++;
        }
        prefixCount[i] = prefixCount[i - 1] + factors;
    }
    initialized = 1;
}

long long maxRounds(int a, int b) {
    if (!initialized) precompute();
    return prefixCount[a] - prefixCount[b];
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

const MAXN = 500005;
const spf = new Int32Array(MAXN);
const prefixCount = new Float64Array(MAXN); 
let initialized = false;

function precompute() {
    for (let i = 0; i < MAXN; i++) spf[i] = i;
    for (let i = 2; i * i < MAXN; i++) {
        if (spf[i] === i) {
            for (let j = i * i; j < MAXN; j += i) {
                if (spf[j] === j) spf[j] = i;
            }
        }
    }
    prefixCount[0] = 0;
    for (let i = 1; i < MAXN; i++) {
        let factors = 0;
        let temp = i;
        while (temp > 1) {
            temp = (temp / spf[temp]) | 0;
            factors++;
        }
        prefixCount[i] = prefixCount[i - 1] + factors;
    }
    initialized = true;
}

function maxRounds(a, b) {
    if (!initialized) precompute();
    return prefixCount[a] - prefixCount[b];
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION


MAXN = 500005
spf = list(range(MAXN))
prefix_count = [0] * MAXN
initialized = False

def precompute():
    global initialized
    i = 2
    while i * i < MAXN:
        if spf[i] == i:
            for j in range(i * i, MAXN, i):
                if spf[j] == j:
                    spf[j] = i
        i += 1
    
    for i in range(2, MAXN):
        factors = 0
        temp = i
        while temp > 1:
            temp //= spf[temp]
            factors += 1
        prefix_count[i] = prefix_count[i-1] + factors
    initialized = True

def maxRounds(a, b):
    if not initialized:
        precompute()
    return prefix_count[a] - prefix_count[b]

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  