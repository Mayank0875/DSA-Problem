## CPP

### SOLUTION

int minCostToJam(string s) {
    int count0 = 0;
    int count1 = 0;
    for (char c : s) {
        if (c == '0') count0++;
        else count1++;
    }
    
    int n = s.length();
    for (int i = 0; i < n; i++) {
        // If s[i] is '0', we need a '1' in t
        if (s[i] == '0') {
            if (count1 > 0) {
                count1--;
            } else {
                return n - i;
            }
        } 
        // If s[i] is '1', we need a '0' in t
        else {
            if (count0 > 0) {
                count0--;
            } else {
                return n - i;
            }
        }
    }
    return 0;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static int minCostToJam(String s) {
    int count0 = 0;
    int count1 = 0;
    for (char c : s.toCharArray()) {
        if (c == '0') count0++;
        else count1++;
    }
    
    int n = s.length();
    for (int i = 0; i < n; i++) {
        char target = (s.charAt(i) == '0') ? '1' : '0';
        
        if (target == '0') {
            if (count0 > 0) {
                count0--;
            } else {
                return n - i;
            }
        } else {
            if (count1 > 0) {
                count1--;
            } else {
                return n - i;
            }
        }
    }
    return 0;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

int minCostToJam(char* s) {
    int count0 = 0;
    int count1 = 0;
    int n = 0;
    
    // Calculate length and counts
    for (int i = 0; s[i] != '\0'; i++) {
        if (s[i] == '0') count0++;
        else count1++;
        n++;
    }
    
    for (int i = 0; i < n; i++) {
        // If s[i] is '0', we need '1'
        if (s[i] == '0') {
            if (count1 > 0) {
                count1--;
            } else {
                return n - i;
            }
        } 
        // If s[i] is '1', we need '0'
        else {
            if (count0 > 0) {
                count0--;
            } else {
                return n - i;
            }
        }
    }
    return 0;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function minCostToJam(s) {
    let count0 = 0;
    let count1 = 0;
    
    for (let char of s) {
        if (char === '0') count0++;
        else count1++;
    }
    
    const n = s.length;
    for (let i = 0; i < n; i++) {
        // if s[i] is '0', we need a '1'
        if (s[i] === '0') {
            if (count1 > 0) {
                count1--;
            } else {
                return n - i;
            }
        } 
        // if s[i] is '1', we need a '0'
        else {
            if (count0 > 0) {
                count0--;
            } else {
                return n - i;
            }
        }
    }
    return 0;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def minCostToJam(s: str) -> int:
    count0 = s.count('0')
    count1 = s.count('1')
    n = len(s)
    
    for i in range(n):
        # If s[i] is '0', we need a '1'
        if s[i] == '0':
            if count1 > 0:
                count1 -= 1
            else:
                return n - i
        # If s[i] is '1', we need a '0'
        else:
            if count0 > 0:
                count0 -= 1
            else:
                return n - i
    return 0

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  