## CPP

### SOLUTION

vector<int> specialArrangement(vector<int>& nums) {
    vector<int> evens, odds;
    for (int i = 0; i < nums.size(); i++) {
        if (i % 2 == 0) evens.push_back(nums[i]);
        else odds.push_back(nums[i]);
    }
    sort(evens.begin(), evens.end());
    sort(odds.begin(), odds.end(), greater<int>());
    
    vector<int> result(nums.size());
    int e = 0, o = 0;
    for (int i = 0; i < nums.size(); i++) {
        if (i % 2 == 0) result[i] = evens[e++];
        else result[i] = odds[o++];
    }
    return result;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static List<Integer> specialArrangement(List<Integer> nums) {
    List<Integer> evens = new ArrayList<>();
    List<Integer> odds = new ArrayList<>();
    
    for (int i = 0; i < nums.size(); i++) {
        if (i % 2 == 0) evens.add(nums.get(i));
        else odds.add(nums.get(i));
    }
    
    Collections.sort(evens);
    odds.sort(Collections.reverseOrder());
    
    List<Integer> result = new ArrayList<>(nums.size());
    int e = 0, o = 0;
    for (int i = 0; i < nums.size(); i++) {
        if (i % 2 == 0) result.add(evens.get(e++));
        else result.add(odds.get(o++));
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

int* specialArrangement(int* nums, int size) {
    int* evens = (int*)malloc(size * sizeof(int));
    int* odds = (int*)malloc(size * sizeof(int));
    int e = 0, o = 0;

    for (int i = 0; i < size; i++) {
        if (i % 2 == 0) evens[e++] = nums[i];
        else odds[o++] = nums[i];
    }

    qsort(evens, e, sizeof(int), compareAsc);
    qsort(odds, o, sizeof(int), compareDesc);

    int* result = (int*)malloc(size * sizeof(int));
    e = 0, o = 0;
    for (int i = 0; i < size; i++) {
        if (i % 2 == 0) result[i] = evens[e++];
        else result[i] = odds[o++];
    }

    free(evens);
    free(odds);
    return result;
}

int compareAsc(const void* a, const void* b) {
    return (*(int*)a - *(int*)b);
}

int compareDesc(const void* a, const void* b) {
    return (*(int*)b - *(int*)a);
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function specialArrangement(nums) {
    const evens = [];
    const odds = [];
    
    for (let i = 0; i < nums.length; i++) {
        if (i % 2 === 0) evens.push(nums[i]);
        else odds.push(nums[i]);
    }
    
    evens.sort((a, b) => a - b);
    odds.sort((a, b) => b - a);
    
    const result = [];
    let e = 0, o = 0;
    for (let i = 0; i < nums.length; i++) {
        if (i % 2 === 0) result.push(evens[e++]);
        else result.push(odds[o++]);
    }
    return result;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def specialArrangement(nums):
    evens = []
    odds = []
    
    for i in range(len(nums)):
        if i % 2 == 0:
            evens.append(nums[i])
        else:
            odds.append(nums[i])
    
    evens.sort()
    odds.sort(reverse=True)
    
    result = []
    e, o = 0, 0
    for i in range(len(nums)):
        if i % 2 == 0:
            result.append(evens[e])
            e += 1
        else:
            result.append(odds[o])
            o += 1
    return result

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  