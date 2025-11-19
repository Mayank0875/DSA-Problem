## CPP

### SOLUTION

vector<int> findNextLowerTemperature(vector<int>& temps) {
    int n = temps.size();
    vector<int> result(n);
    stack<int> s; 

    for (int i = n - 1; i >= 0; --i) {
        while (!s.empty() && temps[s.top()] >= temps[i]) {
            s.pop();
        }
        if (s.empty()) {
            result[i] = -1;
        } else {
            result[i] = temps[s.top()];
        }
        s.push(i);
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

public static List<Integer> findNextLowerTemperature(List<Integer> temps) {
    int n = temps.size();
    List<Integer> result = new ArrayList<>(Collections.nCopies(n, 0));
    Stack<Integer> s = new Stack<>();

    for (int i = n - 1; i >= 0; --i) {
        while (!s.isEmpty() && temps.get(s.peek()) >= temps.get(i)) {
            s.pop();
        }
        if (s.isEmpty()) {
            result.set(i, -1);
        } else {
            result.set(i, temps.get(s.peek()));
        }
        s.push(i);
    }
    return result;
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

int* findNextLowerTemperature(int* temps, int n) {
    int* result = (int*)malloc(n * sizeof(int));
    int* stack = (int*)malloc(n * sizeof(int));
    int top = -1;

    for (int i = n - 1; i >= 0; --i) {
        while (top >= 0 && temps[stack[top]] >= temps[i]) {
            top--;
        }
        if (top == -1) {
            result[i] = -1;
        } else {
            result[i] = temps[stack[top]];
        }
        stack[++top] = i;
    }

    free(stack);
    return result;
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function findNextLowerTemperature(temps) {
    const n = temps.length;
    const result = new Array(n);
    const stack = [];

    for (let i = n - 1; i >= 0; --i) {
        while (stack.length > 0 && temps[stack[stack.length - 1]] >= temps[i]) {
            stack.pop();
        }
        if (stack.length === 0) {
            result[i] = -1;
        } else {
            result[i] = temps[stack[stack.length - 1]];
        }
        stack.push(i);
    }
    return result;
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def findNextLowerTemperature(temps):
    n = len(temps)
    result = [0] * n
    stack = []

    for i in range(n - 1, -1, -1):
        while stack and temps[stack[-1]] >= temps[i]:
            stack.pop()
        if not stack:
            result[i] = -1
        else:
            result[i] = temps[stack[-1]]
        stack.append(i)

    return result


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  