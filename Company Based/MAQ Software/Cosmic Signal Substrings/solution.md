## CPP

### SOLUTION

int Solver(string p) {
    int ans=1,prev_ans=1;
    vector<int> arr(26,0);
    arr[p[0]-'a']=1;
    for (int i=1;i<p.size();i++){
        if ((p[i-1]-'a'+1)%26==p[i]-'a') // Checking for continuation
            prev_ans++;
        else
            prev_ans=1;
        if (arr[p[i]-'a']<prev_ans){
            ans+=prev_ans-arr[p[i]-'a'];
            arr[p[i]-'a']=prev_ans;
        }
    }
    return ans;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static int Solver(String p) {
    int ans = 1, prevAns = 1;
    int[] arr = new int[26];
    arr[p.charAt(0) - 'a'] = 1;

    for (int i = 1; i < p.length(); i++) {
        if ((p.charAt(i - 1) - 'a' + 1) % 26 == (p.charAt(i) - 'a'))
            prevAns++;
        else
            prevAns = 1;

        int idx = p.charAt(i) - 'a';
        if (arr[idx] < prevAns) {
            ans += prevAns - arr[idx];
            arr[idx] = prevAns;
        }
    }
    return ans;
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

int Solver(const char* p) {
    int ans = 1, prev_ans = 1;
    int arr[26] = {0};
    arr[p[0] - 'a'] = 1;

    for (int i = 1; p[i] != '\0'; i++) {
        if (((p[i - 1] - 'a' + 1) % 26) == (p[i] - 'a'))
            prev_ans++;
        else
            prev_ans = 1;

        int idx = p[i] - 'a';
        if (arr[idx] < prev_ans) {
            ans += prev_ans - arr[idx];
            arr[idx] = prev_ans;
        }
    }
    return ans;
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function Solver(p) {
    let ans = 1, prevAns = 1;
    let arr = new Array(26).fill(0);
    arr[p.charCodeAt(0) - 97] = 1;

    for (let i = 1; i < p.length; i++) {
        if ((p.charCodeAt(i - 1) - 97 + 1) % 26 === (p.charCodeAt(i) - 97))
            prevAns++;
        else
            prevAns = 1;

        let idx = p.charCodeAt(i) - 97;
        if (arr[idx] < prevAns) {
            ans += prevAns - arr[idx];
            arr[idx] = prevAns;
        }
    }
    return ans;
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def Solver(p):
    ans = 1
    prev_ans = 1
    arr = [0] * 26
    arr[ord(p[0]) - ord('a')] = 1

    for i in range(1, len(p)):
        if (ord(p[i - 1]) - ord('a') + 1) % 26 == ord(p[i]) - ord('a'):
            prev_ans += 1
        else:
            prev_ans = 1

        idx = ord(p[i]) - ord('a')
        if arr[idx] < prev_ans:
            ans += prev_ans - arr[idx]
            arr[idx] = prev_ans
    return ans


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  