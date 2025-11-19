## CPP

### SOLUTION

vector<int> findNextHigherAttendance(vector<int>& attendance) {
    int n = attendance.size();
    vector<int> result(n);
    stack<int> s; 

    for (int i = n - 1; i >= 0; --i) {
        while (!s.empty() && attendance[s.top()] <= attendance[i]) {
            s.pop();
        }
        if (s.empty()) {
            result[i] = -1;
        } else {
            result[i] = attendance[s.top()];
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

public static List<Integer> findNextHigherAttendance(List<Integer> attendance) {
    int n = attendance.size();
    List<Integer> result = new ArrayList<>(Collections.nCopies(n, 0));
    Stack<Integer> s = new Stack<>();

    for (int i = n - 1; i >= 0; --i) {
        while (!s.isEmpty() && attendance.get(s.peek()) <= attendance.get(i)) {
            s.pop();
        }
        if (s.isEmpty()) {
            result.set(i, -1);
        } else {
            result.set(i, attendance.get(s.peek()));
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

int* findNextHigherAttendance(int* attendance, int n) {
    int* result = (int*)malloc(n * sizeof(int));
    int* stack = (int*)malloc(n * sizeof(int));
    int top = -1;

    for (int i = n - 1; i >= 0; --i) {
        while (top >= 0 && attendance[stack[top]] <= attendance[i]) {
            top--;
        }
        if (top == -1) {
            result[i] = -1;
        } else {
            result[i] = attendance[stack[top]];
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

function findNextHigherAttendance(attendance) {
    const n = attendance.length;
    const result = new Array(n);
    const stack = [];

    for (let i = n - 1; i >= 0; --i) {
        while (stack.length > 0 && attendance[stack[stack.length - 1]] <= attendance[i]) {
            stack.pop();
        }
        if (stack.length === 0) {
            result[i] = -1;
        } else {
            result[i] = attendance[stack[stack.length - 1]];
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

def findNextHigherAttendance(attendance):
    n = len(attendance)
    result = [0] * n
    stack = []

    for i in range(n - 1, -1, -1):
        while stack and attendance[stack[-1]] <= attendance[i]:
            stack.pop()
        if not stack:
            result[i] = -1
        else:
            result[i] = attendance[stack[-1]]
        stack.append(i)

    return result



### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  