## CPP

### SOLUTION

bool check(long long max_sum, int n, int k,vector<int>& x) {
    int required_scribes = 1;
    long long current_sum = 0;
    for (int pages : x) {
        if (pages > max_sum) { 
            return false;
        }
        if (current_sum + pages <= max_sum) {
            current_sum += pages;
        } else {
            required_scribes++;
            current_sum = pages;
        }
    }
    return required_scribes <= k;
}

long long AncientScrolls(int n, int k, vector<int> &x) {
    long long total_sum = 0;
    int max_single = 0;
    for (int i = 0; i < n; ++i) {
        total_sum += x[i];
        max_single = max(max_single, x[i]);
    }

    long long low = max_single; 
    long long high = total_sum;
    long long ans = high;

    while (low <= high) {
        long long mid = low + (high - low) / 2;
        if (check(mid, n, k, x)) {
            ans = mid;
            high = mid - 1;
        } else {
            low = mid + 1;
        }
    }
    return ans;
}



### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## JAVA

### SOLUTION

public class Main {
    static boolean check(long maxSum, int n, int k, List<Integer> x) {
        int requiredScribes = 1;
        long currentSum = 0;
        for (int pages : x) {
            if (pages > maxSum) return false;
            if (currentSum + pages <= maxSum) {
                currentSum += pages;
            } else {
                requiredScribes++;
                currentSum = pages;
            }
        }
        return requiredScribes <= k;
    }

    public static long AncientScrolls(int n, int k, List<Integer> x) {
        long totalSum = 0;
        int maxSingle = 0;
        for (int pages : x) {
            totalSum += pages;
            maxSingle = Math.max(maxSingle, pages);
        }

        long low = maxSingle;
        long high = totalSum;
        long ans = high;

        while (low <= high) {
            long mid = low + (high - low) / 2;
            if (check(mid, n, k, x)) {
                ans = mid;
                high = mid - 1;
            } else {
                low = mid + 1;
            }
        }
        return ans;
    }
}

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## C

### SOLUTION


#include <stdbool.h>

bool check(long long max_sum, int n, int k, int x[]) {
    int required_scribes = 1;
    long long current_sum = 0;
    for (int i = 0; i < n; i++) {
        int pages = x[i];
        if (pages > max_sum) return false;
        if (current_sum + pages <= max_sum) {
            current_sum += pages;
        } else {
            required_scribes++;
            current_sum = pages;
        }
    }
    return required_scribes <= k;
}

long long AncientScrolls(int n, int k, int x[]) {
    long long total_sum = 0;
    int max_single = 0;
    for (int i = 0; i < n; i++) {
        total_sum += x[i];
        if (x[i] > max_single) max_single = x[i];
    }

    long long low = max_single;
    long long high = total_sum;
    long long ans = high;

    while (low <= high) {
        long long mid = low + (high - low) / 2;
        if (check(mid, n, k, x)) {
            ans = mid;
            high = mid - 1;
        } else {
            low = mid + 1;
        }
    }
    return ans;
}

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## JAVASCRIPT

### SOLUTION

function check(maxSum, n, k, x) {
    let requiredScribes = 1;
    let currentSum = 0n;
    for (let pages of x) {
        let p = BigInt(pages);
        if (p > maxSum) return false;
        if (currentSum + p <= maxSum) {
            currentSum += p;
        } else {
            requiredScribes++;
            currentSum = p;
        }
    }
    return requiredScribes <= k;
}

function AncientScrolls(n, k, x) {
    let totalSum = 0n;
    let maxSingle = 0n;
    for (let pages of x) {
        let p = BigInt(pages);
        totalSum += p;
        if (p > maxSingle) maxSingle = p;
    }

    let low = maxSingle;
    let high = totalSum;
    let ans = high;

    while (low <= high) {
        let mid = low + (high - low) / 2n;
        if (check(mid, n, k, x)) {
            ans = mid;
            high = mid - 1n;
        } else {
            low = mid + 1n;
        }
    }
    return ans;
}

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## PYTHON

### SOLUTION

def check(max_sum: int, n: int, k: int, x: list[int]) -> bool:
    required_scribes = 1
    current_sum = 0
    for pages in x:
        if pages > max_sum:
            return False
        if current_sum + pages <= max_sum:
            current_sum += pages
        else:
            required_scribes += 1
            current_sum = pages
    return required_scribes <= k


def AncientScrolls(n: int, k: int, x: list[int]) -> int:
    total_sum = sum(x)
    max_single = max(x)
    low, high = max_single, total_sum
    ans = high

    while low <= high:
        mid = (low + high) // 2
        if check(mid, n, k, x):
            ans = mid
            high = mid - 1
        else:
            low = mid + 1
    return ans

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256
