## CPP

### SOLUTION

int solve(int n, const vector<int>& x) {
    if (n == 0) return 0;
    
    vector<int> tails;
    for (int val : x) {
        auto it = lower_bound(tails.begin(), tails.end(), val);
        if (it == tails.end()) {
            tails.push_back(val);
        } else {
            *it = val;
        }
    }
    return tails.size();
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static int solve(int n, int[] x) {
    if (n == 0) return 0;
    
    List<Integer> tails = new ArrayList<>();
    
    for (int val : x) {
        // Binary search for the first element >= val
        int left = 0, right = tails.size();
        while (left < right) {
            int mid = left + (right - left) / 2;
            if (tails.get(mid) < val) {
                left = mid + 1;
            } else {
                right = mid;
            }
        }
        
        if (left == tails.size()) {
            tails.add(val);
        } else {
            tails.set(left, val);
        }
    }
    return tails.size();
}
### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  

