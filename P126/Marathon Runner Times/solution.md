## CPP

### SOLUTION

int countStudents(vector<int>& startTime, vector<int>& endTime, int queryStart, int queryEnd) {
    int count = 0;
    int n = startTime.size();
    for (int i = 0; i < n; i++) {
        if (startTime[i] <= queryEnd && endTime[i] >= queryStart) {
            count++;
        }
    }
    return count;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static int countStudents(int[] startTime, int[] endTime, int queryStart, int queryEnd) {
    int count = 0;
    for (int i = 0; i < startTime.length; i++) {
        if (startTime[i] <= queryEnd && endTime[i] >= queryStart) {
            count++;
        }
    }
    return count;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

int countStudents(int* startTime, int startTimeSize, int* endTime, int endTimeSize, int queryStart, int queryEnd) {
    int count = 0;
    for (int i = 0; i < startTimeSize; i++) {
        // Check for overlap
        if (startTime[i] <= queryEnd && endTime[i] >= queryStart) {
            count++;
        }
    }
    return count;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function countStudents(startTime, endTime, queryStart, queryEnd) {
    let count = 0;
    for (let i = 0; i < startTime.length; i++) {
        // Check for overlap
        if (startTime[i] <= queryEnd && endTime[i] >= queryStart) {
            count++;
        }
    }
    return count;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def countStudents(startTime: list, endTime: list, queryStart: int, queryEnd: int) -> int:
    count = 0
    for s, e in zip(startTime, endTime):
        # Check for overlap
        if s <= queryEnd and e >= queryStart:
            count += 1
    return count
### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  