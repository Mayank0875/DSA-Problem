## CPP

### SOLUTION

string isValid(string& s) {
    int balance = 0;
    int returnsToZero = 0;
    
    for (char c : s) {
        if (c == '(') {
            balance++;
        } else {
            balance--;
        }
        
        if (balance == 0) {
            returnsToZero++;
        }
    }
    return ((returnsToZero > 1) ? "Yes" : "No");
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static String isValid(String s) {
    int balance = 0;
    int returnsToZero = 0;

    for (int i = 0; i < s.length(); i++) {
        char c = s.charAt(i);

        if (c == '(') {
            balance++;
        } else {
            balance--;
        }

        if (balance == 0) {
            returnsToZero++;
        }
    }

    return (returnsToZero > 1) ? "Yes" : "No";
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

const char* isValid(char* s) {
    int balance = 0;
    int returnsToZero = 0;

    for (int i = 0; s[i] != '\0'; i++) {
        if (s[i] == '(') {
            balance++;
        } else {
            balance--;
        }

        if (balance == 0) {
            returnsToZero++;
        }
    }

    return (returnsToZero > 1) ? "Yes" : "No";
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function isValid(s) {
    let balance = 0;
    let returnsToZero = 0;

    for (const c of s) {
        if (c === '(') {
            balance++;
        } else {
            balance--;
        }

        if (balance === 0) {
            returnsToZero++;
        }
    }

    return (returnsToZero > 1) ? "Yes" : "No";
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def isValid(s):
    balance = 0
    returnsToZero = 0

    for c in s:
        if c == '(':
            balance += 1
        else:
            balance -= 1

        if balance == 0:
            returnsToZero += 1

    return "Yes" if returnsToZero > 1 else "No"



### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  