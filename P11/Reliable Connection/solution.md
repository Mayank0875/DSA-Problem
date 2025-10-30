## CPP

### SOLUTION

int longestStableSegment(vector<int>& stream, int k) {
    int n = stream.size();
    int left = 0;
    int zero_count = 0;
    int max_len = 0;

    for (int right = 0; right < n; ++right) {
        if (stream[right] == 0) {
            zero_count++;
        }
        while (zero_count > k) {
            if (stream[left] == 0) {
                zero_count--;
            }
            left++;
        }
        max_len = max(max_len, right - left + 1);
    }

    return max_len;
}


### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## JAVA

### SOLUTION

public static int longestStableSegment(int[] stream, int k) {
    int n = stream.length;
    int left = 0;
    int zero_count = 0;
    int max_len = 0;

    for (int right = 0; right < n; ++right) {
        if (stream[right] == 0) {
            zero_count++;
        }
        while (zero_count > k) {
            if (stream[left] == 0) {
                zero_count--;
            }
            left++;
        }
        max_len = Math.max(max_len, right - left + 1);
    }

    return max_len;
}


### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## C

### SOLUTION

int longestStableSegment(int* stream, int n, int k) {
    int left = 0;
    int zero_count = 0;
    int max_len = 0;

    for (int right = 0; right < n; ++right) {
        if (stream[right] == 0) {
            zero_count++;
        }
        while (zero_count > k) {
            if (stream[left] == 0) {
                zero_count--;
            }
            left++;
        }
        if (max_len < right - left + 1) {
            max_len = right - left + 1;
        }
    }

    return max_len;
}

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## JAVASCRIPT

### SOLUTION

function longestStableSegment(stream, k) {
    let n = stream.length;
    let left = 0;
    let zero_count = 0;
    let max_len = 0;

    for (let right = 0; right < n; ++right) {
        if (stream[right] === 0) {
            zero_count++;
        }
        while (zero_count > k) {
            if (stream[left] === 0) {
                zero_count--;
            }
            left++;
        }
        max_len = Math.max(max_len, right - left + 1);
    }

    return max_len;
}

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## PYTHON

### SOLUTION


def longestStableSegment(stream, k):
    n = len(stream)
    left = 0
    zero_count = 0
    max_len = 0

    for right in range(n):
        if stream[right] == 0:
            zero_count += 1
        while zero_count > k:
            if stream[left] == 0:
                zero_count -= 1
            left += 1
        max_len = max(max_len, right - left + 1)

    return max_len

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256
