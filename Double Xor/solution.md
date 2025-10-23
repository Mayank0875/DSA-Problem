## CPP

### SOLUTION

int XorofXoR(vector<int> &arr, int k){
    int n = arr.size();
    int res = 0, l = 0, cur = 0;

    for(int r = 0; r < n; ++r){
        cur ^= arr[r];

        if(r - l + 1 == k){
                    cout << cur << endl;
            res ^= cur;
            cur ^= arr[l];
            l++;
        }
    }

    return res;
}


### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## JAVA

### SOLUTION

public static int XorofXoR(int[] arr, int k) {
    int n = arr.length;
    int res = 0, l = 0, cur = 0;

    for (int r = 0; r < n; ++r) {
        cur ^= arr[r];

        if (r - l + 1 == k) {
            res ^= cur;
            cur ^= arr[l];
            l++;
        }
    }

    return res;
}


### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## C

### SOLUTION

int XorofXoR(int* arr, int n, int k) {
    int res = 0, l = 0, cur = 0;

    for (int r = 0; r < n; ++r) {
        cur ^= arr[r];

        if (r - l + 1 == k) {
            res ^= cur;
            cur ^= arr[l];
            l++;
        }
    }

    return res;
}

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## JAVASCRIPT

### SOLUTION

function XorofXoR(arr, k) {
    const n = arr.length;
    let res = 0, l = 0, cur = 0;

    for (let r = 0; r < n; ++r) {
        cur ^= arr[r];

        if (r - l + 1 === k) {
            res ^= cur;
            cur ^= arr[l];
            l++;
        }
    }

    return res;
}

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## PYTHON

### SOLUTION


def XorofXoR(arr: List[int], k: int) -> int:
    n = len(arr)
    res = 0
    l = 0
    cur = 0

    for r in range(n):
        cur ^= arr[r]

        if r - l + 1 == k:
            res ^= cur
            cur ^= arr[l]
            l += 1

    return res

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256
