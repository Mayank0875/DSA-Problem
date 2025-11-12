## CPP

### SOLUTION

string checkIfPangram(string sentence) {
    vector<bool> seen(26, false);
    int count = 0;
    
    for (char c : sentence) {
        int index = c - 'a';
        if (!seen[index]) {
            seen[index] = true;
            count++;
        }
    }
    
    if (count == 26) {
        return "Yes";
    } else {
        return "No";
    }
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static String checkIfPangram(String sentence) {
    boolean[] seen = new boolean[26];
    int count = 0;

    for (char c : sentence.toCharArray()) {
        int index = c - 'a';
        if (!seen[index]) {
            seen[index] = true;
            count++;
        }
    }

    if (count == 26) {
        return "Yes";
    } else {
        return "No";
    }
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION


char* checkIfPangram(char* sentence) {
    bool seen[26] = {false};
    int count = 0;

    for (int i = 0; i < strlen(sentence); i++) {
        int index = sentence[i] - 'a';
        if (!seen[index]) {
            seen[index] = true;
            count++;
        }
    }

    if (count == 26) {
        return "Yes";
    } else {
        return "No";
    }
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function checkIfPangram(sentence) {
    const seen = new Array(26).fill(false);
    let count = 0;

    for (const c of sentence) {
        const index = c.charCodeAt(0) - 'a'.charCodeAt(0);
        if (!seen[index]) {
            seen[index] = true;
            count++;
        }
    }

    return count === 26 ? "Yes" : "No";
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def checkIfPangram(sentence):
    seen = [False] * 26
    count = 0

    for c in sentence:
        index = ord(c) - ord('a')
        if not seen[index]:
            seen[index] = True
            count += 1

    return "Yes" if count == 26 else "No"

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  