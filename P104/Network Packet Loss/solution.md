## CPP

### SOLUTION

int longestConsecutiveRun(vector<int>& rungs) {
    unordered_set<int> numSet(rungs.begin(), rungs.end());
    int longest = 0;

    for (int num : numSet) {
        // Only start counting if 'num' is the start of a sequence
        if (numSet.find(num - 1) == numSet.end()) {
            int length = 1;

            while (numSet.find(num + length) != numSet.end()) {
                length++;
            }

            longest = max(longest, length);
        }
    }

    return longest;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static int longestConsecutiveRun(int[] rungs) {
    Set<Integer> numSet = new HashSet<>();
    for (int num : rungs) {
        numSet.add(num);
    }

    int longest = 0;

    for (int num : numSet) {
        if (!numSet.contains(num - 1)) {
            int length = 1;

            while (numSet.contains(num + length)) {
                length++;
            }

            longest = Math.max(longest, length);
        }
    }

    return longest;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

int compare(const void* a, const void* b) {
    int int_a = *((int*)a);
    int int_b = *((int*)b);
    if (int_a < int_b) return -1;
    if (int_a > int_b) return 1;
    return 0;
}

int longestConsecutiveRun(int* rungs, int rungsSize) {
    if (rungsSize == 0) return 0;
    
    qsort(rungs, rungsSize, sizeof(int), compare);
    
    int longest = 1;
    int currentStreak = 1;
    
    for (int i = 1; i < rungsSize; i++) {
        if (rungs[i] != rungs[i-1]) {
            if (rungs[i] == rungs[i-1] + 1) {
                currentStreak++;
            } else {
                if (currentStreak > longest) {
                    longest = currentStreak;
                }
                currentStreak = 1;
            }
        }
    }
    
    return (currentStreak > longest) ? currentStreak : longest;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function longestConsecutiveRun(rungs) {
    const numSet = new Set(rungs);
    let longest = 0;

    for (const num of numSet) {
        if (!numSet.has(num - 1)) {
            let length = 1;

            while (numSet.has(num + length)) {
                length++;
            }

            longest = Math.max(longest, length);
        }
    }

    return longest;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def longestConsecutiveRun(rungs: list) -> int:
    num_set = set(rungs)
    longest = 0

    for n in num_set:
        if n - 1 not in num_set:
            length = 1
            while n + length in num_set:
                length += 1
            longest = max(longest, length)
    
    return longest

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  