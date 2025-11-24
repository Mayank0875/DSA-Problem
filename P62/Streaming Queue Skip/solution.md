## CPP

### SOLUTION

int findLeastNumOfUniqueInts(vector<int>& arr, int k) {
    unordered_map<int, int> counts;
    for (int x : arr) {
        counts[x]++;
    }
    
    vector<int> frequencies;
    for (auto& p : counts) {
        frequencies.push_back(p.second);
    }
    
    sort(frequencies.begin(), frequencies.end());
    
    int removedTypes = 0;
    for (int count : frequencies) {
        if (k >= count) {
            k -= count;
            removedTypes++;
        } else {
            break;
        }
    }
    
    return frequencies.size() - removedTypes;
}

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## JAVA

### SOLUTION

public static int findLeastNumOfUniqueInts(int[] arr, int k) {
    Map<Integer, Integer> counts = new HashMap<>();
    for (int x : arr) {
        counts.put(x, counts.getOrDefault(x, 0) + 1);
    }

    List<Integer> frequencies = new ArrayList<>(counts.values());
    Collections.sort(frequencies);

    int removedTypes = 0;
    for (int count : frequencies) {
        if (k >= count) {
            k -= count;
            removedTypes++;
        } else {
            break;
        }
    }

    return frequencies.size() - removedTypes;
}

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## C

### SOLUTION


int compare(const void* a, const void* b) {
    return (*(int*)a - *(int*)b);
}

int findLeastNumOfUniqueInts(int* arr, int n, int k) {
    int* freq = (int*)calloc(100001, sizeof(int)); // Assuming values are within a reasonable range
    for (int i = 0; i < n; i++) {
        freq[arr[i]]++;
    }

    int* frequencies = (int*)malloc(n * sizeof(int));
    int freqSize = 0;
    for (int i = 0; i < 100001; i++) {
        if (freq[i] > 0) {
            frequencies[freqSize++] = freq[i];
        }
    }

    qsort(frequencies, freqSize, sizeof(int), compare);

    int removedTypes = 0;
    for (int i = 0; i < freqSize; i++) {
        if (k >= frequencies[i]) {
            k -= frequencies[i];
            removedTypes++;
        } else {
            break;
        }
    }

    free(freq);
    free(frequencies);

    return freqSize - removedTypes;
}

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## JAVASCRIPT

### SOLUTION

function findLeastNumOfUniqueInts(arr, k) {
    const counts = new Map();
    for (const x of arr) {
        counts.set(x, (counts.get(x) || 0) + 1);
    }

    const frequencies = Array.from(counts.values());
    frequencies.sort((a, b) => a - b);

    let removedTypes = 0;
    for (const count of frequencies) {
        if (k >= count) {
            k -= count;
            removedTypes++;
        } else {
            break;
        }
    }

    return frequencies.length - removedTypes;
}

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## PYTHON

### SOLUTION

def findLeastNumOfUniqueInts(arr, k):
    from collections import Counter
    counts = Counter(arr)
    frequencies = sorted(counts.values())

    removed_types = 0
    for count in frequencies:
        if k >= count:
            k -= count
            removed_types += 1
        else:
            break

    return len(frequencies) - removed_types

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256
