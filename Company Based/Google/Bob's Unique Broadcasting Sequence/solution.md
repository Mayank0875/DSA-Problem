## CPP

### SOLUTION

long long countDistinctSubarrays(std::vector<int>& nums) {
    long long n = nums.size();
    std::map<int, int> fre;
    int l = 0;
    long long res = 0;
    
    for (int r = 0; r < n; ++r) {
        fre[nums[r]]++;
        
        while (fre.size() < (r - l + 1)) {
            fre[nums[l]]--;
            if (fre[nums[l]] == 0) {
                fre.erase(nums[l]);
            }
            l++;
        }
        
        res += (r - l + 1);
    }
    
    return res;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public long countDistinctSubarrays(int[] nums) {
    int n = nums.length;
    Map<Integer, Integer> fre = new HashMap<>();
    int l = 0;
    long res = 0;
    
    for (int r = 0; r < n; r++) {
        fre.put(nums[r], fre.getOrDefault(nums[r], 0) + 1);
        
        while (fre.size() < (r - l + 1)) {
            fre.put(nums[l], fre.get(nums[l]) - 1);
            if (fre.get(nums[l]) == 0) {
                fre.remove(nums[l]);
            }
            l++;
        }
        
        res += (r - l + 1);
    }
    
    return res;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

// Helper structure for coordinate compression
typedef struct {
    int val;
    int originalIdx;
} Pair;

int cmp(const void* a, const void* b) {
    return ((Pair*)a)->val - ((Pair*)b)->val;
}

long long countDistinctSubarrays(int* nums, int numsSize) {
    if (numsSize == 0) return 0;

    // Coordinate Compression
    Pair* p = (Pair*)malloc(numsSize * sizeof(Pair));
    for(int i = 0; i < numsSize; i++) {
        p[i].val = nums[i];
        p[i].originalIdx = i;
    }
    
    qsort(p, numsSize, sizeof(Pair), cmp);
    
    // Map large values to 0..numsSize-1 in a new array
    int* compressed = (int*)malloc(numsSize * sizeof(int));
    int rank = 0;
    compressed[p[0].originalIdx] = rank;
    
    for(int i = 1; i < numsSize; i++) {
        if (p[i].val != p[i-1].val) {
            rank++;
        }
        compressed[p[i].originalIdx] = rank;
    }
    free(p);
    
    // Sliding window using array frequency
    int* fre = (int*)calloc(numsSize + 1, sizeof(int));
    int l = 0;
    long long res = 0;
    int uniqueCount = 0;
    
    for (int r = 0; r < numsSize; r++) {
        int val = compressed[r];
        if (fre[val] == 0) uniqueCount++;
        fre[val]++;
        
        while (uniqueCount < (r - l + 1)) {
            int leftVal = compressed[l];
            fre[leftVal]--;
            if (fre[leftVal] == 0) uniqueCount--;
            l++;
        }
        
        res += (long long)(r - l + 1);
    }
    
    free(compressed);
    free(fre);
    return res;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function countDistinctSubarrays(nums) {
    let n = nums.length;
    let fre = new Map();
    let l = 0;
    let res = 0;
    
    for (let r = 0; r < n; r++) {
        fre.set(nums[r], (fre.get(nums[r]) || 0) + 1);
        
        while (fre.size < (r - l + 1)) {
            let count = fre.get(nums[l]);
            if (count === 1) {
                fre.delete(nums[l]);
            } else {
                fre.set(nums[l], count - 1);
            }
            l++;
        }
        
        res += (r - l + 1);
    }
    
    return res;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def countDistinctSubarrays(nums):
    n = len(nums)
    fre = {}
    l = 0
    res = 0
    
    for r in range(n):
        fre[nums[r]] = fre.get(nums[r], 0) + 1
        
        while len(fre) < (r - l + 1):
            fre[nums[l]] -= 1
            if fre[nums[l]] == 0:
                del fre[nums[l]]
            l += 1
            
        res += (r - l + 1)
        
    return res

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  