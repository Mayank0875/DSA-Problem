## CPP

### SOLUTION

int scoreOfParentheses(string s) {
    int score=0;

    int open_count=0; 

    for(int i=0;i<s.size();i++){
        if(s[i]==')') open_count--;
        else{
            open_count++;
        }
        if(s[i]==')' && s[i-1]=='(') score+=pow(2,open_count);
    }
    return score;
    
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static int scoreOfParentheses(String s) {
    int score = 0;
    int openCount = 0;

    for (int i = 0; i < s.length(); i++) {
        if (s.charAt(i) == ')') openCount--;
        else openCount++;

        if (s.charAt(i) == ')' && s.charAt(i - 1) == '(')
            score += (int)Math.pow(2, openCount);
    }
    return score;
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION


int scoreOfParentheses(char *s) {
    int score = 0;
    int open_count = 0;

    for (int i = 0; s[i] != '\0'; i++) {
        if (s[i] == ')') open_count--;
        else open_count++;

        if (s[i] == ')' && s[i - 1] == '(')
            score += (int)pow(2, open_count);
    }
    return score;
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function scoreOfParentheses(s) {
    let score = 0;
    let openCount = 0;

    for (let i = 0; i < s.length; i++) {
        if (s[i] === ')') openCount--;
        else openCount++;

        if (s[i] === ')' && s[i - 1] === '(')
            score += Math.pow(2, openCount);
    }
    return score;
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def scoreOfParentheses(s: str) -> int:
    score = 0
    open_count = 0

    for i in range(len(s)):
        if s[i] == ')':
            open_count -= 1
        else:
            open_count += 1

        if s[i] == ')' and s[i - 1] == '(':
            score += pow(2, open_count)

    return score


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  