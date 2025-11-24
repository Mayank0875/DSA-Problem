## CPP

### SOLUTION

long long countStarPairs(vector<int>& luminosity, int target) {
    unordered_map<int, int> freq;
    long long count = 0;
    for (int star : luminosity) {
        int complement = target - star;
        if (freq.find(complement) != freq.end()) {
            count += freq[complement];
        }
        freq[star]++;
    }
    return count;
}


### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## JAVA

### SOLUTION

public static long countStarPairs(int[] luminosity, int target) {
    Map<Integer, Integer> freq = new HashMap<>();
    long count = 0;

    for (int star : luminosity) {
        int complement = target - star;
        if (freq.containsKey(complement)) {
            count += freq.get(complement);
        }
        freq.put(star, freq.getOrDefault(star, 0) + 1);
    }

    return count;
}


### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## C

### SOLUTION

long long countStarPairs(int* luminosity, int n, int target) {
    int* freq = (int*)calloc(100001, sizeof(int)); // Assuming luminosity values are within a reasonable range
    long long count = 0;

    for (int i = 0; i < n; i++) {
        int complement = target - luminosity[i];
        if (complement >= 0 && complement <= 100000) {
            count += freq[complement];
        }
        freq[luminosity[i]]++;
    }

    free(freq);
    return count;
}

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## JAVASCRIPT

### SOLUTION

function countStarPairs(luminosity, target) {
    const freq = new Map();
    let count = 0;

    for (const star of luminosity) {
        const complement = target - star;
        if (freq.has(complement)) {
            count += freq.get(complement);
        }
        freq.set(star, (freq.get(star) || 0) + 1);
    }

    return count;
}


### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## PYTHON

### SOLUTION

def countStarPairs(luminosity, target):
    freq = {}
    count = 0

    for star in luminosity:
        complement = target - star
        if complement in freq:
            count += freq[complement]
        freq[star] = freq.get(star, 0) + 1

    return count

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256
