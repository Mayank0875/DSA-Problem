## CPP

### SOLUTION
int findMaxLength(vector<int>& nums) {
    int n = nums.size();
    int max_length = 0;
    int count = 0;
    map<int, int> map;
    map[0] = -1;

    for (int i = 0; i < n; ++i) {
        if (nums[i] == 0) {
            count--;
        } else {
            count++;
        }

        if (map.count(count)) {
            max_length = max(max_length, i - map[count]);
        } else {
            map[count] = i;
        }
    }

    return max_length;
}

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## JAVA

### SOLUTION

import java.util.*;

public class Main {
    public static int findMaxLength(int[] nums) {
        int n = nums.length;
        int max_length = 0;
        int count = 0;
        Map<Integer, Integer> map = new HashMap<>();
        map.put(0, -1);

        for (int i = 0; i < n; ++i) {
            if (nums[i] == 0) {
                count--;
            } else {
                count++;
            }

            if (map.containsKey(count)) {
                max_length = Math.max(max_length, i - map.get(count));
            } else {
                map.put(count, i);
            }
        }

        return max_length;
    }
}


### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## C

### SOLUTION

int findMaxLength(int* nums, int n) {
    int max_length = 0;
    int count = 0;

    int size = 4 * n + 10;
    int *map = (int*)malloc(size * sizeof(int));
    for (int i = 0; i < size; i++) map[i] = INT_MIN;

    int shift = 2 * n;
    map[shift + 0] = -1;

    for (int i = 0; i < n; ++i) {
        if (nums[i] == 0)
            count--;
        else
            count++;

        if (map[shift + count] != INT_MIN) {
            int len = i - map[shift + count];
            if (len > max_length)
                max_length = len;
        } else {
            map[shift + count] = i;
        }
    }

    free(map);
    return max_length;
}

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## JAVASCRIPT

### SOLUTION

function findMaxLength(nums) {
    const n = nums.length;
    let max_length = 0;
    let count = 0;
    const map = new Map();
    map.set(0, -1);

    for (let i = 0; i < n; ++i) {
        if (nums[i] === 0) {
            count--;
        } else {
            count++;
        }

        if (map.has(count)) {
            max_length = Math.max(max_length, i - map.get(count));
        } else {
            map.set(count, i);
        }
    }

    return max_length;
}

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## PYTHON

### SOLUTION

def findMaxLength(nums):
    n = len(nums)
    max_length = 0
    count = 0
    mp = {0: -1}

    for i in range(n):
        if nums[i] == 0:
            count -= 1
        else:
            count += 1

        if count in mp:
            max_length = max(max_length, i - mp[count])
        else:
            mp[count] = i

    return max_length

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256
