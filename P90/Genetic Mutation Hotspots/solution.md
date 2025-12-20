## CPP

### SOLUTION

long long countSubarrays(int n, int k, std::vector<int>& arr) {
    std::map<int, int> mp;
    int l = 0;
    long long res = 0;
    
    for(int r = 0; r < n; ++r) {
        mp[arr[r]]++;
        
        while(mp.size() > k) {
            mp[arr[l]]--;
            if(mp[arr[l]] == 0) {
                mp.erase(arr[l]);
            }
            l++;
        }
        
        res += (long long)(r - l + 1);
    }
    
    return res;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static long countSubarrays(int n, int k, int[] arr) {
    HashMap<Integer, Integer> map = new HashMap<>();
    int l = 0;
    long res = 0;
    
    for (int r = 0; r < n; r++) {
        map.put(arr[r], map.getOrDefault(arr[r], 0) + 1);
        
        while (map.size() > k) {
            map.put(arr[l], map.get(arr[l]) - 1);
            if (map.get(arr[l]) == 0) {
                map.remove(arr[l]);
            }
            l++;
        }
        
        res += (r - l + 1);
    }
    
    return res;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  

