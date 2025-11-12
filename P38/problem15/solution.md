## CPP

### SOLUTION

vector<int> findPreviousLowerPrice(vector<int>& prices) {
    int n = prices.size();
    vector<int> result(n);
    stack<int> s; 

    for (int i = 0; i < n; ++i) {
        while (!s.empty() && prices[s.top()] >= prices[i]) {
            s.pop();
        }
        if (s.empty()) {
            result[i] = -1;
        } else {
            result[i] = prices[s.top()];
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

public static List<Integer> findPreviousLowerPrice(List<Integer> prices) {
    int n = prices.size();
    List<Integer> result = new ArrayList<>(Collections.nCopies(n, 0));
    Stack<Integer> s = new Stack<>();

    for (int i = 0; i < n; ++i) {
        while (!s.isEmpty() && prices.get(s.peek()) >= prices.get(i)) {
            s.pop();
        }
        if (s.isEmpty()) {
            result.set(i, -1);
        } else {
            result.set(i, prices.get(s.peek()));
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

int* findPreviousLowerPrice(int* prices, int n) {
    int* result = (int*)malloc(n * sizeof(int));
    int* stack = (int*)malloc(n * sizeof(int));
    int top = -1;

    for (int i = 0; i < n; ++i) {
        while (top >= 0 && prices[stack[top]] >= prices[i]) {
            top--;
        }
        if (top == -1) {
            result[i] = -1;
        } else {
            result[i] = prices[stack[top]];
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

function findPreviousLowerPrice(prices) {
    const n = prices.length;
    const result = new Array(n);
    const stack = [];

    for (let i = 0; i < n; ++i) {
        while (stack.length > 0 && prices[stack[stack.length - 1]] >= prices[i]) {
            stack.pop();
        }
        if (stack.length === 0) {
            result[i] = -1;
        } else {
            result[i] = prices[stack[stack.length - 1]];
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

def findPreviousLowerPrice(prices):
    n = len(prices)
    result = [0] * n
    stack = []

    for i in range(n):
        while stack and prices[stack[-1]] >= prices[i]:
            stack.pop()
        if not stack:
            result[i] = -1
        else:
            result[i] = prices[stack[-1]]
        stack.append(i)

    return result

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  