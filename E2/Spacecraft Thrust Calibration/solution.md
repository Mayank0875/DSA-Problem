## CPP

### SOLUTION
bool threeSquaresTarget(vector<long long> cards, long long target) {
    int n = (int)cards.size();
    for (int i = 0; i < n; ++i) cards[i] = cards[i] * cards[i];
    sort(cards.begin(), cards.end());
    for (int i = 0; i < n; ++i) {
        long long need = target - cards[i];
        int l = i + 1, r = n - 1;
        while (l < r) {
            long long s = cards[l] + cards[r];
            if (s == need) return true;
            if (s < need) ++l; else --r;
        }
    }
    return false;
}

### METADATA
**TimeLimit**
1000

**MemoryLimit**
256

## JAVA

### SOLUTION
public static boolean threeSquaresTarget(long[] cards, long target) {
    int n = cards.length;
    for (int i = 0; i < n; i++) cards[i] = cards[i] * cards[i];
    java.util.Arrays.sort(cards);
    for (int i = 0; i < n; i++) {
        long need = target - cards[i];
        int l = i + 1, r = n - 1;
        while (l < r) {
            long s = cards[l] + cards[r];
            if (s == need) return true;
            if (s < need) l++; else r--;
        }
    }
    return false;
}

### METADATA
**TimeLimit**
1000

**MemoryLimit**
256

## C

### SOLUTION
int threeSquaresTarget(long long* cards, int n, long long target) {
    for (int i = 0; i < n; ++i) cards[i] = cards[i] * cards[i];
    // qsort comparator for long long
    int cmp_ll(const void* x, const void* y);
    qsort(cards, n, sizeof(long long), cmp_ll);
    for (int i = 0; i < n; ++i) {
        long long need = target - cards[i];
        int l = i + 1, r = n - 1;
        while (l < r) {
            long long s = cards[l] + cards[r];
            if (s == need) return 1;
            if (s < need) ++l; else --r;
        }
    }
    return 0;
}

// Provide comparator definition outside function
int cmp_ll(const void* x, const void* y) {
    long long a = *(const long long*)x;
    long long b = *(const long long*)y;
    if (a < b) return -1; if (a > b) return 1; return 0;
}

### METADATA
**TimeLimit**
1000

**MemoryLimit**
256

## JAVASCRIPT

### SOLUTION
function threeSquaresTarget(cards, target) {
    const a = cards.map(x => x * x).sort((x, y) => x - y);
    const n = a.length;
    for (let i = 0; i < n; i++) {
        const need = target - a[i];
        let l = i + 1, r = n - 1;
        while (l < r) {
            const s = a[l] + a[r];
            if (s === need) return true;
            if (s < need) l++; else r--;
        }
    }
    return false;
}

### METADATA
**TimeLimit**
1000

**MemoryLimit**
256

## PYTHON

### SOLUTION
def three_squares_target(cards: List[int], target: int) -> bool:
    sq = [x*x for x in cards]
    sq.sort()
    n = len(sq)
    for i in range(n):
        need = target - sq[i]
        l, r = i+1, n-1
        while l < r:
            s = sq[l] + sq[r]
            if s == need:
                return True
            if s < need:
                l += 1
            else:
                r -= 1
    return False

### METADATA
**TimeLimit**
1000

**MemoryLimit**
256