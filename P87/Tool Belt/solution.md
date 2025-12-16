## CPP

### SOLUTION

int solve(string s) {
    bool seen_one = false;
    bool in_zero_block = false;
    int ans = 0;

    for (char c : s) {
        if (c == '1') {
            if (in_zero_block) {
                ans++;
                in_zero_block = false;
            }
            seen_one = true;
        } else { // c == '0'
            if (seen_one) {
                in_zero_block = true;
            }
        }
    }
    if (in_zero_block) {
        ans++;
    }
    return ans;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static int solve(String s) {
    boolean seenOne = false;
    boolean inZeroBlock = false;
    int ans = 0;

    for (int i = 0; i < s.length(); i++) {
        char c = s.charAt(i);
        if (c == '1') {
            if (inZeroBlock) {
                ans++;
                inZeroBlock = false;
            }
            seenOne = true;
        } else { // c == '0'
            if (seenOne) {
                inZeroBlock = true;
            }
        }
    }
    if (inZeroBlock) {
        ans++;
    }
    return ans;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  

