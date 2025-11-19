## CPP

### SOLUTION

vector<int> calculateSpans(vector<int>& prices) {
    int n = prices.size();
    vector<int> spans(n);
    stack<int> s;

    for (int i = 0; i < n; ++i) {
        while (!s.empty() && prices[s.top()] <= prices[i]) {
            s.pop();
        }
        spans[i] = (s.empty()) ? (i + 1) : (i - s.top());

        s.push(i);
    }
    return spans;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static List<Integer> calculateSpans(List<Integer> prices) {
    int n = prices.size();
    List<Integer> spans = new ArrayList<>(Collections.nCopies(n, 0));
    Stack<Integer> s = new Stack<>();

    for (int i = 0; i < n; ++i) {
        while (!s.isEmpty() && prices.get(s.peek()) <= prices.get(i)) {
            s.pop();
        }
        spans.set(i, s.isEmpty() ? (i + 1) : (i - s.peek()));
        s.push(i);
    }
    return spans;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

int* calculateSpans(int* prices, int n) {
    int* spans = (int*)malloc(n * sizeof(int));
    int* stack = (int*)malloc(n * sizeof(int));
    int top = -1;

    for (int i = 0; i < n; ++i) {
        while (top >= 0 && prices[stack[top]] <= prices[i]) {
            top--;
        }
        spans[i] = (top == -1) ? (i + 1) : (i - stack[top]);
        stack[++top] = i;
    }

    free(stack);
    return spans;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function calculateSpans(prices) {
    const n = prices.length;
    const spans = new Array(n);
    const stack = [];

    for (let i = 0; i < n; ++i) {
        while (stack.length > 0 && prices[stack[stack.length - 1]] <= prices[i]) {
            stack.pop();
        }
        spans[i] = stack.length === 0 ? (i + 1) : (i - stack[stack.length - 1]);
        stack.push(i);
    }
    return spans;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def calculateSpans(prices):
    n = len(prices)
    spans = [0] * n
    stack = []

    for i in range(n):
        while stack and prices[stack[-1]] <= prices[i]:
            stack.pop()
        spans[i] = (i + 1) if not stack else (i - stack[-1])
        stack.append(i)
    return spans

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  