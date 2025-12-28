## CPP

### SOLUTION

string isValid(string& s) {
    stack<char> st;
    unordered_map<char, char> mapping = {{')', '('}, {']', '['}, {'}', '{'}};

    for (char c : s) {
        if (mapping.count(c)) {
            if (st.empty() || st.top() != mapping[c]) {
                return "No";
            }
            st.pop();
        } else {
            st.push(c);
        }
    }
    return (st.empty() ? "Yes" : "No");
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static String isValid(String s) {
    Stack<Character> st = new Stack<>();
    Map<Character, Character> mapping = new HashMap<>();
    mapping.put(')', '(');
    mapping.put(']', '[');
    mapping.put('}', '{');

    for (char c : s.toCharArray()) {
        if (mapping.containsKey(c)) {
            if (st.isEmpty() || st.peek() != mapping.get(c)) {
                return "No";
            }
            st.pop();
        } else {
            st.push(c);
        }
    }
    return st.isEmpty() ? "Yes" : "No";
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

const char* isValid(char* s) {
    int MAX = 1000000;
    char stack[MAX];
    int top = -1;

    for (int i = 0; s[i] != '\0'; i++) {
        char c = s[i];
        if (c == '(' || c == '[' || c == '{') {
            stack[++top] = c;
        } else if (c == ')' || c == ']' || c == '}') {
            if (top == -1)
                return "No";
            char open = stack[top--];
            if ((c == ')' && open != '(') ||
                (c == ']' && open != '[') ||
                (c == '}' && open != '{')) {
                return "No";
            }
        }
    }
    return (top == -1) ? "Yes" : "No";
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function isValid(s) {
    const st = [];
    const mapping = { ')': '(', ']': '[', '}': '{' };

    for (const c of s) {
        if (mapping[c]) {
            if (st.length === 0 || st[st.length - 1] !== mapping[c]) {
                return "No";
            }
            st.pop();
        } else {
            st.push(c);
        }
    }
    return st.length === 0 ? "Yes" : "No";
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def isValid(s):
    st = []
    mapping = {')': '(', ']': '[', '}': '{'}

    for c in s:
        if c in mapping:
            if not st or st[-1] != mapping[c]:
                return "No"
            st.pop()
        else:
            st.append(c)

    return "Yes" if not st else "No"


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  