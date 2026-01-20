## CPP

### SOLUTION

bool checkMatch(stack<char>& stk, string& part, int partLength) {
    stack<char> temp = stk;
    for (int partIndex = partLength - 1; partIndex >= 0; partIndex--) {
        if (temp.top() != part[partIndex]) {
            return false;
        }
        temp.pop();
    }
    return true;
}

string removeOccurrences(string s, string part) {
    stack<char> stk;
    int strLength = s.length();
    int partLength = part.length();

    for (int index = 0; index < strLength; index++) {
        stk.push(s[index]);

        if (stk.size() >= partLength && checkMatch(stk, part, partLength)) {
            for (int j = 0; j < partLength; j++) {
                stk.pop();
            }
        }
    }

    string result = "";
    while (!stk.empty()) {
        result = stk.top() + result;
        stk.pop();
    }

    return result;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public String removeOccurrences(String s, String part) {
    // Using StringBuilder as a stack of characters for efficiency
    StringBuilder sb = new StringBuilder();
    int partLength = part.length();

    for (char c : s.toCharArray()) {
        sb.append(c);
        
        // Check if the suffix of the current string matches 'part'
        if (sb.length() >= partLength) {
            boolean match = true;
            // Check match from right to left
            for (int i = 0; i < partLength; i++) {
                if (sb.charAt(sb.length() - 1 - i) != part.charAt(partLength - 1 - i)) {
                    match = false;
                    break;
                }
            }
            
            if (match) {
                // Pop 'partLength' characters
                sb.setLength(sb.length() - partLength);
            }
        }
    }
    
    return sb.toString();
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

char* removeOccurrences(char* s, char* part) {
    int n = strlen(s);
    int m = strlen(part);
    // Stack implemented as a char array
    char* stk = (char*)malloc((n + 1) * sizeof(char));
    int top = 0; // Points to the next empty slot
    
    for (int i = 0; i < n; i++) {
        stk[top++] = s[i];
        
        if (top >= m) {
            bool match = true;
            for (int j = 0; j < m; j++) {
                if (stk[top - 1 - j] != part[m - 1 - j]) {
                    match = false;
                    break;
                }
            }
            
            if (match) {
                top -= m; // Pop by reducing the index
            }
        }
    }
    
    stk[top] = '\0';
    return stk;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

var removeOccurrences = function(s, part) {
    const stk = [];
    const partLen = part.length;
    
    for (let char of s) {
        stk.push(char);
        
        if (stk.length >= partLen) {
            let match = true;
            for (let i = 0; i < partLen; i++) {
                if (stk[stk.length - 1 - i] !== part[partLen - 1 - i]) {
                    match = false;
                    break;
                }
            }
            
            if (match) {
                for (let i = 0; i < partLen; i++) {
                    stk.pop();
                }
            }
        }
    }
    
    return stk.join('');
};

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def removeOccurrences(s: str, part: str) -> str:
    stk = []
    part_len = len(part)
    
    for char in s:
        stk.append(char)
        
        # Check if valid length and suffix matches part
        if len(stk) >= part_len:
            # Compare suffix
            match = True
            for i in range(part_len):
                if stk[-(i+1)] != part[-(i+1)]:
                    match = False
                    break
            
            if match:
                # Pop part_len times
                for _ in range(part_len):
                    stk.pop()
                    
    return "".join(stk)

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  