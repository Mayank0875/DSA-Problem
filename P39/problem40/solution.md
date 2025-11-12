## CPP

### SOLUTION

vector<int> findPreviousTallerBuilding(vector<int>& heights) {
    int n = heights.size();
    vector<int> result(n);
    stack<int> s;

    for (int i = 0; i < n; ++i) {
        while (!s.empty() && heights[s.top()] <= heights[i]) {
            s.pop();
        }
        if (s.empty()) {
            result[i] = -1;
        } else {
            result[i] = heights[s.top()];
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

public static List<Integer> findPreviousTallerBuilding(List<Integer> heights) {
    int n = heights.size();
    List<Integer> result = new ArrayList<>(Collections.nCopies(n, 0));
    Stack<Integer> s = new Stack<>();

    for (int i = 0; i < n; ++i) {
        while (!s.isEmpty() && heights.get(s.peek()) <= heights.get(i)) {
            s.pop();
        }
        if (s.isEmpty()) {
            result.set(i, -1);
        } else {
            result.set(i, heights.get(s.peek()));
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

int* findPreviousTallerBuilding(int* heights, int n) {
    int* result = (int*)malloc(n * sizeof(int));
    int* stack = (int*)malloc(n * sizeof(int));
    int top = -1;

    for (int i = 0; i < n; ++i) {
        while (top >= 0 && heights[stack[top]] <= heights[i]) {
            top--;
        }
        if (top == -1) {
            result[i] = -1;
        } else {
            result[i] = heights[stack[top]];
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

function findPreviousTallerBuilding(heights) {
    const n = heights.length;
    const result = new Array(n);
    const stack = [];

    for (let i = 0; i < n; ++i) {
        while (stack.length > 0 && heights[stack[stack.length - 1]] <= heights[i]) {
            stack.pop();
        }
        if (stack.length === 0) {
            result[i] = -1;
        } else {
            result[i] = heights[stack[stack.length - 1]];
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

def findPreviousTallerBuilding(heights):
    n = len(heights)
    result = [0] * n
    stack = []

    for i in range(n):
        while stack and heights[stack[-1]] <= heights[i]:
            stack.pop()
        if not stack:
            result[i] = -1
        else:
            result[i] = heights[stack[-1]]
        stack.append(i)

    return result


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  