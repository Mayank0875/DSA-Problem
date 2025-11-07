## CPP

### SOLUTION

static bool compare(int a, int b) {
    if (__builtin_popcount(a) == __builtin_popcount(b)) {
        return a < b;
    }
    
    return __builtin_popcount(a) < __builtin_popcount(b);
}

vector<int> sortByBits(vector<int>& arr) {
    sort(arr.begin(), arr.end(), compare);
    return arr;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static int[] sortByBits(int[] arr) {
    Integer[] nums = Arrays.stream(arr).boxed().toArray(Integer[]::new);
    Comparator<Integer> comparator = new CustomComparator();
    Arrays.sort(nums, comparator);
    return Arrays.stream(nums).mapToInt(Integer::intValue).toArray();
}

class CustomComparator implements Comparator<Integer> {
    @Override
    public int compare(Integer a, Integer b) {
        if (Integer.bitCount(a) == Integer.bitCount(b)) {
            return a - b;
        }
        
        return Integer.bitCount(a) - Integer.bitCount(b);
    }
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

int countBits(int x) {
    int cnt = 0;
    while (x) {
        cnt += x & 1;
        x >>= 1;
    }
    return cnt;
}

int compare(const void* a, const void* b) {
    int x = *(int*)a;
    int y = *(int*)b;
    int bx = countBits(x);
    int by = countBits(y);

    if (bx == by)
        return x - y;
    return bx - by;
}

void sortByBits(int* arr, int n) {
    qsort(arr, n, sizeof(int), compare);
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function sortByBits(arr) {
    arr.sort((a, b) => {
        const bitA = a.toString(2).split('1').length - 1;
        const bitB = b.toString(2).split('1').length - 1;
        if (bitA === bitB) return a - b;
        return bitA - bitB;
    });
    return arr;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def sortByBits(arr: List[int]) -> List[int]:
    arr.sort(key = lambda num: (num.bit_count(), num))
    return arr

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  