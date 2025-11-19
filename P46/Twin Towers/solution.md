## CPP

### SOLUTION
vector<long long> Numbers(vector<long long>& numbers) {
    unordered_map<long long,int> freq;
    for (auto v : numbers) ++freq[v];
    vector<long long> out;
    out.reserve(freq.size());
    for (auto &p : freq) if (p.second == 2) out.push_back(p.first);
    sort(out.begin(), out.end());
    return out;
}

### METADATA
**TimeLimit**
1000

**MemoryLimit**
256

## JAVA

### SOLUTION
public static long[] Numbers(long[] numbers) {
    java.util.HashMap<Long,Integer> map = new java.util.HashMap<>();
    for (long v : numbers) map.put(v, map.getOrDefault(v, 0) + 1);
    java.util.ArrayList<Long> list = new java.util.ArrayList<>();
    for (java.util.Map.Entry<Long,Integer> e : map.entrySet()) if (e.getValue() == 2) list.add(e.getKey());
    java.util.Collections.sort(list);
    long[] res = new long[list.size()];
    for (int i=0;i<list.size();i++) res[i] = list.get(i);
    return res;
}

### METADATA
**TimeLimit**
1000

**MemoryLimit**
256

## C

### SOLUTION
// Simple approach: sort a copy and scan counts, then collect values with count==2.
static int cmp_ll(const void* x, const void* y){
    long long a = *(const long long*)x, b = *(const long long*)y;
    return (a<b)?-1:(a>b); 
}
void Numbers(const long long* numbers, int n, long long** out, int* m) {
    long long* b = (long long*)malloc(sizeof(long long)*n);
    for(int i=0;i<n;i++) b[i]=numbers[i];
    qsort(b, n, sizeof(long long), cmp_ll);
    long long* tmp = (long long*)malloc(sizeof(long long)*n);
    int k=0;
    for(int i=0;i<n;){
        int j=i; while(j<n && b[j]==b[i]) j++;
        if (j-i==2) tmp[k++]=b[i];
        i=j;
    }
    *out = (long long*)malloc(sizeof(long long)*k);
    memcpy(*out, tmp, sizeof(long long)*k);
    *m = k;
    free(tmp); free(b);
}

### METADATA
**TimeLimit**
1000

**MemoryLimit**
256

## JAVASCRIPT

### SOLUTION
function Numbers(numbers) {
    const mp = new Map();
    for (const v of numbers) mp.set(v, (mp.get(v)||0)+1);
    const ans = [];
    for (const [k,c] of mp) if (c===2) ans.push(k);
    ans.sort((x,y)=>x-y);
    return ans;
}

### METADATA
**TimeLimit**
1000

**MemoryLimit**
256

## PYTHON

### SOLUTION
def Numbers(numbers: List[int]) -> List[int]:
    from collections import Counter
    cnt = Counter(numbers)
    out = [x for x,c in cnt.items() if c==2]
    out.sort()
    return out

### METADATA
**TimeLimit**
1000

**MemoryLimit**
256