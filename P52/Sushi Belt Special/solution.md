## CPP

### SOLUTION

vector<int> frequencySort(vector<int>& nums) {
    unordered_map<int, int> counts;
    for (int x : nums) {
        counts[x]++;
    }
    
    sort(nums.begin(), nums.end(), [&](int a, int b) {
        if (counts[a] != counts[b]) {
            return counts[a] < counts[b];
        }
        return a > b;
    });
    
    return nums;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static List<Integer> frequencySort(List<Integer> nums) {
    Map<Integer, Integer> counts = new HashMap<>();
    for (int x : nums) {
        counts.put(x, counts.getOrDefault(x, 0) + 1);
    }

    nums.sort((a, b) -> {
        if (!counts.get(a).equals(counts.get(b))) {
            return counts.get(a) - counts.get(b);
        }
        return b - a;
    });

    return nums;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

#include <stdio.h>
#include <stdlib.h>

typedef struct {
    int value;
    int freq;
} Pair;

int compare(const void* a, const void* b) {
    Pair* p1 = (Pair*)a;
    Pair* p2 = (Pair*)b;

    if (p1->freq != p2->freq)
        return p1->freq - p2->freq;

    return p2->value - p1->value;
}

int* frequencySort(int* nums, int n) {
    int counts[201] = {0};

    for (int i = 0; i < n; i++)
        counts[nums[i] + 100]++;

    Pair* arr = (Pair*)malloc(n * sizeof(Pair));
    int* result = (int*)malloc(n * sizeof(int));

    for (int i = 0; i < n; i++) {
        arr[i].value = nums[i];
        arr[i].freq = counts[nums[i] + 100];
    }

    qsort(arr, n, sizeof(Pair), compare);

    for (int i = 0; i < n; i++)
        result[i] = arr[i].value;

    free(arr);
    return result;
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function frequencySort(nums) {
    const counts = new Map();
    nums.forEach(x => counts.set(x, (counts.get(x) || 0) + 1));

    nums.sort((a, b) => {
        if (counts.get(a) !== counts.get(b)) {
            return counts.get(a) - counts.get(b);
        }
        return b - a;
    });

    return nums;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def frequencySort(nums):
    from collections import Counter
    counts = Counter(nums)

    nums.sort(key=lambda x: (counts[x], -x))
    return nums

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  