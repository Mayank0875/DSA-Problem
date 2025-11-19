## CPP

### SOLUTION

long long largestRectangleArea(vector<int>& heights) {
    stack<int> s; 
    long long max_area = 0;
    int n = heights.size();
    vector<int> h(n + 1);
    for(int i = 0; i < n; ++i) h[i] = heights[i];
    h[n] = 0; 

    for (int i = 0; i <= n; ++i) {
        while (!s.empty() && h[s.top()] >= h[i]) {
            long long height = h[s.top()];
            s.pop();
            long long width = s.empty() ? i : i - s.top() - 1;
            max_area = max(max_area, height * width);
        }
        s.push(i);
    }
    return max_area;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static long largestRectangleArea(List<Integer> heights) {
    Stack<Integer> s = new Stack<>();
    long maxArea = 0;
    int n = heights.size();
    List<Integer> h = new ArrayList<>(heights);
    h.add(0);

    for (int i = 0; i <= n; ++i) {
        while (!s.isEmpty() && h.get(s.peek()) >= h.get(i)) {
            long height = h.get(s.pop());
            long width = s.isEmpty() ? i : i - s.peek() - 1;
            maxArea = Math.max(maxArea, height * width);
        }
        s.push(i);
    }
    return maxArea;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

long long largestRectangleArea(int* heights, int n) {
    long long maxArea = 0;
    int* stack = (int*)malloc((n + 1) * sizeof(int));
    int* h = (int*)malloc((n + 1) * sizeof(int));
    int top = -1;

    for (int i = 0; i < n; ++i) h[i] = heights[i];
    h[n] = 0;

    for (int i = 0; i <= n; ++i) {
        while (top >= 0 && h[stack[top]] >= h[i]) {
            long long height = h[stack[top--]];
            long long width = (top == -1) ? i : i - stack[top] - 1;
            long long area = height * width;
            if (area > maxArea) maxArea = area;
        }
        stack[++top] = i;
    }

    free(stack);
    free(h);
    return maxArea;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function largestRectangleArea(heights) {
    const n = heights.length;
    const h = [...heights, 0];
    const stack = [];
    let maxArea = 0;

    for (let i = 0; i <= n; ++i) {
        while (stack.length > 0 && h[stack[stack.length - 1]] >= h[i]) {
            const height = h[stack.pop()];
            const width = stack.length === 0 ? i : i - stack[stack.length - 1] - 1;
            maxArea = Math.max(maxArea, height * width);
        }
        stack.push(i);
    }
    return maxArea;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def largestRectangleArea(heights):
    n = len(heights)
    h = heights + [0]
    stack = []
    max_area = 0

    for i in range(n + 1):
        while stack and h[stack[-1]] >= h[i]:
            height = h[stack.pop()]
            width = i if not stack else i - stack[-1] - 1
            max_area = max(max_area, height * width)
        stack.append(i)

    return max_area

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  