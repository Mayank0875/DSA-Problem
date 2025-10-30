## CPP

### SOLUTION
int sameFreq(vector<int>& marks) {
    int cnt[101] = {0};
    for (int v : marks) ++cnt[v];
    int best = 0;
    for (int m=0;m<=100;++m) best = max(best, cnt[m]);
    return best;
}

### METADATA
**TimeLimit**
1000

**MemoryLimit**
256

## JAVA

### SOLUTION
public static int sameFreq(int[] marks) {
    int[] cnt = new int[101];
    for (int v : marks) cnt[v]++;
    int best = 0;
    for (int m=0;m<=100;m++) if (cnt[m] > best) best = cnt[m];
    return best;
}

### METADATA
**TimeLimit**
1000

**MemoryLimit**
256

## C

### SOLUTION
int sameFreq(const int* marks, int n) {
    int cnt[101] = {0};
    for (int i=0;i<n;i++) cnt[marks[i]]++;
    int best = 0;
    for (int m=0;m<=100;m++) if (cnt[m] > best) best = cnt[m];
    return best;
}

### METADATA
**TimeLimit**
1000

**MemoryLimit**
256

## JAVASCRIPT

### SOLUTION
function sameFreq(marks) {
    const cnt = Array(101).fill(0);
    for (const v of marks) cnt[v]++;
    let best = 0;
    for (let m=0;m<=100;m++) if (cnt[m] > best) best = cnt[m];
    return best;
}

### METADATA
**TimeLimit**
1000

**MemoryLimit**
256

## PYTHON

### SOLUTION
def sameFreq(marks: List[int]) -> int:
    cnt = [0]*101
    for v in marks: cnt[v] += 1
    return max(cnt)

### METADATA
**TimeLimit**
1000

**MemoryLimit**
256