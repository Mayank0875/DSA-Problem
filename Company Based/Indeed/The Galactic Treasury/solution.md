## CPP
### SOLUTION
vector<int> sumEvenAfterQueries(vector<int>& nums, vector<vector<int>>& queries) {
    int sumEven = 0;
    for (int x : nums) {
        if (x % 2 == 0) {
            sumEven += x;
        }
    }
    
    vector<int> ans;
    ans.reserve(queries.size());
    
    for (auto& q : queries) {
        int val = q[0];
        int index = q[1];
        
        if (nums[index] % 2 == 0) {
            sumEven -= nums[index];
        }
        
        nums[index] += val;
        
        if (nums[index] % 2 == 0) {
            sumEven += nums[index];
        }
        
        ans.push_back(sumEven);
    }
    
    return ans;
}

### METADATA
**TimeLimit**
1000
**MemoryLimit**
256000

## JAVA
### SOLUTION
public static int[] sumEvenAfterQueries(int[] nums, int[][] queries) {
    int sumEven = 0;
    for (int x : nums) {
        if (x % 2 == 0) {
            sumEven += x;
        }
    }
    
    int[] ans = new int[queries.length];
    
    for (int i = 0; i < queries.length; ++i) {
        int val = queries[i][0];
        int index = queries[i][1];
        
        if (nums[index] % 2 == 0) {
            sumEven -= nums[index];
        }
        
        nums[index] += val;
        
        if (nums[index] % 2 == 0) {
            sumEven += nums[index];
        }
        
        ans[i] = sumEven;
    }
    
    return ans;
}

### METADATA
**TimeLimit**
1000
**MemoryLimit**
256000

## C
### SOLUTION
int* sumEvenAfterQueries(int* nums, int numsSize, int** queries, int queriesSize, int* queriesColSize, int* returnSize) {
    int sumEven = 0;
    for (int i = 0; i < numsSize; i++) {
        if (nums[i] % 2 == 0) {
            sumEven += nums[i];
        }
    }
    
    int* ans = (int*)malloc(queriesSize * sizeof(int));
    *returnSize = queriesSize;
    
    for (int i = 0; i < queriesSize; i++) {
        int val = queries[i][0];
        int index = queries[i][1];
        
        if (nums[index] % 2 == 0) {
            sumEven -= nums[index];
        }
        
        nums[index] += val;
        
        if (nums[index] % 2 == 0) {
            sumEven += nums[index];
        }
        
        ans[i] = sumEven;
    }
    
    return ans;
}

### METADATA
**TimeLimit**
1000
**MemoryLimit**
256000

## JAVASCRIPT
### SOLUTION
function sumEvenAfterQueries(nums, queries) {
    let sumEven = 0;
    for (let x of nums) {
        if (x % 2 === 0) {
            sumEven += x;
        }
    }
    
    let ans = [];
    
    for (let i = 0; i < queries.length; i++) {
        let val = queries[i][0];
        let index = queries[i][1];
        
        if (nums[index] % 2 === 0) {
            sumEven -= nums[index];
        }
        
        nums[index] += val;
        
        if (nums[index] % 2 === 0) {
            sumEven += nums[index];
        }
        
        ans.push(sumEven);
    }
    
    return ans;
}

### METADATA
**TimeLimit**
1000
**MemoryLimit**
256000

## PYTHON
### SOLUTION
def sum_even_after_queries(nums: list[int], queries: list[list[int]]) -> list[int]:
    sum_even = sum(x for x in nums if x % 2 == 0)
    ans = []
    
    for val, index in queries:
        if nums[index] % 2 == 0:
            sum_even -= nums[index]
        
        nums[index] += val
        
        if nums[index] % 2 == 0:
            sum_even += nums[index]
        
        ans.append(sum_even)
        
    return ans

### METADATA
**TimeLimit**
1000
**MemoryLimit**
256000