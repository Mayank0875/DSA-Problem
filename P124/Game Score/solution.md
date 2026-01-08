## CPP

### SOLUTION

bool checkSubarraySum(vector<int>& nums, int k) {
    long long prefixMod = 0;
    unordered_map<int, int> modSeen;
    modSeen[0] = -1;

    for (int i = 0; i < nums.size(); i++) {
        prefixMod = (prefixMod + nums[i]) % k;

        if (modSeen.find(prefixMod) != modSeen.end()) {
            // ensures that the size of subarray is at least 2
            if (i - modSeen[prefixMod] > 1) {
                return true;
            }
        } else {
            // mark the value of prefixMod with the current index.
            modSeen[prefixMod] = i;
        }
    }

    return false;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static boolean checkSubarraySum(int[] nums, int k) {
    long prefixMod = 0;
    Map<Integer, Integer> modSeen = new HashMap<>();
    modSeen.put(0, -1);

    for (int i = 0; i < nums.length; i++) {
        prefixMod = (prefixMod + nums[i]) % k;
        // In Java, modulo of negative numbers can be negative, 
        // though input constraints say nums[i] >= 0, so prefixMod >= 0.
        
        int mod = (int) prefixMod;

        if (modSeen.containsKey(mod)) {
            if (i - modSeen.get(mod) > 1) {
                return true;
            }
        } else {
            modSeen.put(mod, i);
        }
    }

    return false;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

typedef struct {
    int key;
    int val;
    int used; // 0 for empty, 1 for occupied
} HashEntry;

// Simple Open Addressing Hash Map
int get_hash_index(int key, int size) {
    int idx = key % size;
    if (idx < 0) idx += size;
    return idx;
}

void insert(HashEntry* table, int size, int key, int val) {
    int idx = get_hash_index(key, size);
    while (table[idx].used) {
        if (table[idx].key == key) return; // Already exists, don't update for this problem
        idx = (idx + 1) % size;
    }
    table[idx].key = key;
    table[idx].val = val;
    table[idx].used = 1;
}

int find_val(HashEntry* table, int size, int key) {
    int idx = get_hash_index(key, size);
    while (table[idx].used) {
        if (table[idx].key == key) return table[idx].val;
        idx = (idx + 1) % size;
    }
    return -2; // Sentinel for not found
}

bool checkSubarraySum(int* nums, int numsSize, int k) {
    if (numsSize < 2) return false;

    // Table size: power of 2 roughly 2 * numsSize for load factor 0.5
    int tableSize = 1;
    while (tableSize <= numsSize * 2) tableSize <<= 1;
    
    HashEntry* map = (HashEntry*)calloc(tableSize, sizeof(HashEntry));
    
    // Initialize map with base case: mod 0 at index -1
    insert(map, tableSize, 0, -1);
    
    long long prefixMod = 0;
    bool found = false;
    
    for (int i = 0; i < numsSize; i++) {
        prefixMod = (prefixMod + nums[i]) % k;
        int mod = (int)prefixMod;
        
        int prevIndex = find_val(map, tableSize, mod);
        
        if (prevIndex != -2) {
            if (i - prevIndex > 1) {
                found = true;
                break;
            }
        } else {
            insert(map, tableSize, mod, i);
        }
    }
    
    free(map);
    return found;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function checkSubarraySum(nums, k) {
    let prefixMod = 0;
    const modSeen = new Map();
    modSeen.set(0, -1);

    for (let i = 0; i < nums.length; i++) {
        prefixMod = (prefixMod + nums[i]) % k;

        if (modSeen.has(prefixMod)) {
            if (i - modSeen.get(prefixMod) > 1) {
                return true;
            }
        } else {
            modSeen.set(prefixMod, i);
        }
    }

    return false;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def checkSubarraySum(nums: list, k: int) -> bool:
    prefix_mod = 0
    mod_seen = {0: -1}
    
    for i, num in enumerate(nums):
        prefix_mod = (prefix_mod + num) % k
        
        if prefix_mod in mod_seen:
            if i - mod_seen[prefix_mod] > 1:
                return True
        else:
            mod_seen[prefix_mod] = i
            
    return False

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  