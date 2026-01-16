## CPP

### SOLUTION

string solve(string s, string t) {
    vector<int> fs(26, 0), ft(26, 0);
    for (char c : s) fs[c - 'a']++;
    for (char c : t) ft[c - 'a']++;

    for (int i = 0; i < 26; i++) {
        if (fs[i] > ft[i]) return "Impossible";
    }

    string ans = "";
    int p = 0; // pointer for s
    
    for (int i = 0; i < t.size(); i++) {
        for (int j = 0; j < 26; j++) {
            if (ft[j] > 0) {
                if (ft[j] == fs[j] && (p >= s.size() || s[p] != (char)(j + 'a'))) {
                    continue;
                }

                ans += (char)(j + 'a');
                ft[j]--;

                if (p < s.size() && s[p] == ans.back()) {
                    fs[j]--;
                    p++;
                }
                break; 
            }
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

public static String solve(String s, String t) {
    int[] fs = new int[26];
    int[] ft = new int[26];
    for (char c : s.toCharArray()) fs[c - 'a']++;
    for (char c : t.toCharArray()) ft[c - 'a']++;

    for (int i = 0; i < 26; i++) {
        if (fs[i] > ft[i]) return "Impossible";
    }

    StringBuilder ans = new StringBuilder();
    int p = 0;
    int n = t.length();
    int m = s.length();

    for (int i = 0; i < n; i++) {
        for (int j = 0; j < 26; j++) {
            if (ft[j] > 0) {
                char current = (char)('a' + j);
                // Greedy check
                if (ft[j] == fs[j]) {
                    if (p >= m || s.charAt(p) != current) {
                        continue;
                    }
                }

                ans.append(current);
                ft[j]--;

                if (p < m && s.charAt(p) == current) {
                    fs[j]--;
                    p++;
                }
                break;
            }
        }
    }
    return ans.toString();
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

char* solve(char* s, char* t) {
    int fs[26] = {0};
    int ft[26] = {0};
    int slen = strlen(s);
    int tlen = strlen(t);

    for (int i = 0; i < slen; i++) fs[s[i] - 'a']++;
    for (int i = 0; i < tlen; i++) ft[t[i] - 'a']++;

    for (int i = 0; i < 26; i++) {
        if (fs[i] > ft[i]) {
            char* imp = (char*)malloc(11);
            strcpy(imp, "Impossible");
            return imp;
        }
    }

    char* ans = (char*)malloc(tlen + 1);
    int p = 0; // pointer for s
    int k = 0; // pointer for ans

    for (int i = 0; i < tlen; i++) {
        for (int j = 0; j < 26; j++) {
            if (ft[j] > 0) {
                char current = (char)(j + 'a');
                if (ft[j] == fs[j]) {
                    if (p >= slen || s[p] != current) {
                        continue;
                    }
                }

                ans[k++] = current;
                ft[j]--;

                if (p < slen && s[p] == current) {
                    fs[j]--;
                    p++;
                }
                break;
            }
        }
    }
    ans[k] = '\0';
    return ans;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function solve(s, t) {
    const fs = new Array(26).fill(0);
    const ft = new Array(26).fill(0);
    
    for (let char of s) fs[char.charCodeAt(0) - 97]++;
    for (let char of t) ft[char.charCodeAt(0) - 97]++;
    
    for (let i = 0; i < 26; i++) {
        if (fs[i] > ft[i]) return "Impossible";
    }
    
    let ans = "";
    let p = 0;
    const tLen = t.length;
    const sLen = s.length;
    
    for (let i = 0; i < tLen; i++) {
        for (let j = 0; j < 26; j++) {
            if (ft[j] > 0) {
                const current = String.fromCharCode(j + 97);
                if (ft[j] === fs[j]) {
                    if (p >= sLen || s[p] !== current) {
                        continue;
                    }
                }
                
                ans += current;
                ft[j]--;
                
                if (p < sLen && s[p] === current) {
                    fs[j]--;
                    p++;
                }
                break;
            }
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

def solve(s: str, t: str) -> str:
    fs = [0] * 26
    ft = [0] * 26
    
    for char in s:
        fs[ord(char) - ord('a')] += 1
    for char in t:
        ft[ord(char) - ord('a')] += 1
        
    for i in range(26):
        if fs[i] > ft[i]:
            return "Impossible"
            
    ans = []
    p = 0
    t_len = len(t)
    s_len = len(s)
    
    for _ in range(t_len):
        for j in range(26):
            if ft[j] > 0:
                current = chr(j + ord('a'))
                # If we are tight on this char, we MUST use it for a match in s
                if ft[j] == fs[j]:
                    if p >= s_len or s[p] != current:
                        continue
                
                ans.append(current)
                ft[j] -= 1
                
                if p < s_len and s[p] == current:
                    fs[j] -= 1
                    p += 1
                break
                
    return "".join(ans)

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  