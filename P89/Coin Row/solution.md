## CPP

### SOLUTION

string solve(int n) {
    if (n % 4 == 1) {
        return "Fluttershy";
    } else if (n % 4 == 2) {
        return "Pinkie Pie";
    } else if (n % 4 == 3) {
        return "Pinkie Pie";
    } else {
        return "Fluttershy";
    }
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static String solve(int n) {
    int rem = n % 4;
    if (rem == 1) {
        return "Fluttershy";
    } else if (rem == 2) {
        return "Pinkie Pie";
    } else if (rem == 3) {
        return "Pinkie Pie";
    } else {
        return "Fluttershy";
    }
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  

