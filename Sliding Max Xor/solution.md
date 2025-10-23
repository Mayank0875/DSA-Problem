## CPP

### SOLUTION

int SlidingMaxXor(vector<int> &arr, int k){
    int n = arr.size();
    int res = 0;
    deque<int> que;

    int l = 0;
    for(int r = 0; r < n; ++r){
        while(! que.empty() and que.back() < arr[r]){
            que.pop_back();
        }
        que.push_back(arr[r]);

        if(r - l + 1 == k){
            res ^= que.front();
            if(arr[l] == que.front()){
                que.pop_front();
            }
            l++;
        }
    }
    return res;
}


### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## JAVA

### SOLUTION


public static int SlidingMaxXor(int[] arr, int k) {
    int n = arr.length;
    int res = 0;
    Deque<Integer> dq = new ArrayDeque<>();

    for(int i = 0; i < n; i++){
        while(!dq.isEmpty() && arr[dq.peekLast()] <= arr[i])
            dq.pollLast();
        dq.addLast(i);

        if(i >= k - 1){
            res ^= arr[dq.peekFirst()];

            if(dq.peekFirst() == i - k + 1)
                dq.pollFirst();
        }
    }

    return res;
}



### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## C

### SOLUTION

int SlidingMaxXor(int* arr, int n, int k){
    int* dq = (int*)malloc(n * sizeof(int));
    int front = 0, back = -1;
    int res = 0;

    for(int i = 0; i < n; i++){
        while(back >= front && arr[dq[back]] <= arr[i]) back--;
        dq[++back] = i;

        if(i >= k - 1){
            res ^= arr[dq[front]];

            if(dq[front] == i - k + 1) front++;
        }
    }

    free(dq);
    return res;
}

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## JAVASCRIPT

### SOLUTION

function SlidingMaxXor(arr, k) {
    let n = arr.length;
    let dq = [];
    let res = 0;

    for(let i = 0; i < n; i++){
        while(dq.length > 0 && arr[dq[dq.length - 1]] <= arr[i])
            dq.pop();
        dq.push(i);

        if(i >= k - 1){
            res ^= arr[dq[0]];

            if(dq[0] == i - k + 1)
                dq.shift();
        }
    }

    return res;
}


### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## PYTHON

### SOLUTION



def SlidingMaxXor(arr, k):
    dq = deque()
    res = 0

    for i, val in enumerate(arr):
        while dq and arr[dq[-1]] <= val:
            dq.pop()
        dq.append(i)

        if i >= k - 1:
            res ^= arr[dq[0]]

            if dq[0] == i - k + 1:
                dq.popleft()

    return res

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256
