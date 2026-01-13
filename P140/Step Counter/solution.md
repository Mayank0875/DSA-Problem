## CPP

### SOLUTION

vector<int> findKiteRanks(vector<int>& arr) {
    vector<int> sortedArr = arr;
    sort(sortedArr.begin(), sortedArr.end());
    sortedArr.erase(unique(sortedArr.begin(), sortedArr.end()), sortedArr.end());
    
    vector<int> ranks;
    for (int x : arr) {
        ranks.push_back(lower_bound(sortedArr.begin(), sortedArr.end(), x) - sortedArr.begin() + 1);
    }
    return ranks;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static int[] findKiteRanks(int[] arr) {
    int[] sortedArr = arr.clone();
    Arrays.sort(sortedArr);
    
    Map<Integer, Integer> rankMap = new HashMap<>();
    int rank = 1;
    
    for (int num : sortedArr) {
        if (!rankMap.containsKey(num)) {
            rankMap.put(num, rank++);
        }
    }
    
    int[] result = new int[arr.length];
    for (int i = 0; i < arr.length; i++) {
        result[i] = rankMap.get(arr[i]);
    }
    return result;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

struct Element {
    int value;
    int index;
};

int compareElements(const void* a, const void* b) {
    return ((struct Element*)a)->value - ((struct Element*)b)->value;
}

int* findKiteRanks(int* arr, int arrSize, int* returnSize) {
    *returnSize = arrSize;
    if (arrSize == 0) return NULL;

    struct Element* elements = (struct Element*)malloc(arrSize * sizeof(struct Element));
    for (int i = 0; i < arrSize; i++) {
        elements[i].value = arr[i];
        elements[i].index = i;
    }

    qsort(elements, arrSize, sizeof(struct Element), compareElements);

    int* result = (int*)malloc(arrSize * sizeof(int));
    int rank = 1;
    
    result[elements[0].index] = rank;
    for (int i = 1; i < arrSize; i++) {
        if (elements[i].value > elements[i - 1].value) {
            rank++;
        }
        result[elements[i].index] = rank;
    }

    free(elements);
    return result;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function findKiteRanks(arr) {
    const sortedUnique = [...new Set(arr)].sort((a, b) => a - b);
    const rankMap = new Map();
    
    sortedUnique.forEach((val, index) => {
        rankMap.set(val, index + 1);
    });
    
    return arr.map(val => rankMap.get(val));
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def findKiteRanks(arr: list) -> list:
    sorted_unique = sorted(list(set(arr)))
    rank_map = {val: i + 1 for i, val in enumerate(sorted_unique)}
    return [rank_map[x] for x in arr]

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  