## CPP

### SOLUTION

int lengthOfLongestSubstring(string s) {
    vector<int> charIndex(128, -1);
    int maxLength = 0;
    int left = 0;

    for (int right = 0; right < s.length(); right++) {
        char currentChar = s[right];
        if (charIndex[currentChar] >= left) {
            left = charIndex[currentChar] + 1;
        }
        charIndex[currentChar] = right;
        maxLength = max(maxLength, right - left + 1);
    }

    return maxLength;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static int lengthOfLongestSubstring(String s) {
    int[] charIndex = new int[128];
    Arrays.fill(charIndex, -1);
    int maxLength = 0;
    int left = 0;

    for (int right = 0; right < s.length(); right++) {
        char currentChar = s.charAt(right);
        if (charIndex[currentChar] >= left) {
            left = charIndex[currentChar] + 1;
        }
        charIndex[currentChar] = right;
        maxLength = Math.max(maxLength, right - left + 1);
    }

    return maxLength;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

int lengthOfLongestSubstring(char* s) {
    int charIndex[128];
    for (int i = 0; i < 128; i++) {
        charIndex[i] = -1;
    }

    int maxLength = 0;
    int left = 0;

    for (int right = 0; s[right] != '\0'; right++) {
        char currentChar = s[right];
        if (charIndex[currentChar] >= left) {
            left = charIndex[currentChar] + 1;
        }
        charIndex[currentChar] = right;
        int currentLength = right - left + 1;
        if (currentLength > maxLength) {
            maxLength = currentLength;
        }
    }

    return maxLength;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function lengthOfLongestSubstring(s) {
    const charIndex = new Array(128).fill(-1);
    let maxLength = 0;
    let left = 0;

    for (let right = 0; right < s.length; right++) {
        const currentChar = s[right];
        if (charIndex[currentChar.charCodeAt(0)] >= left) {
            left = charIndex[currentChar.charCodeAt(0)] + 1;
        }
        charIndex[currentChar.charCodeAt(0)] = right;
        maxLength = Math.max(maxLength, right - left + 1);
    }

    return maxLength;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def lengthOfLongestSubstring(s):
    char_index = [-1] * 128
    max_length = 0
    left = 0

    for right in range(len(s)):
        current_char = s[right]
        if char_index[ord(current_char)] >= left:
            left = char_index[ord(current_char)] + 1
        char_index[ord(current_char)] = right
        max_length = max(max_length, right - left + 1)

    return max_length

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  