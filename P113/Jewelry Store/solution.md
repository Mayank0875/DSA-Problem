## CPP

### SOLUTION

int countUnluckyApprentices(vector<int>& apprentices, vector<int>& potions) {
    int fireCount = 0;
    int iceCount = 0;

    for (int app : apprentices) {
        if (app == 0) fireCount++;
        else iceCount++;
    }

    for (int potion : potions) {
        if (potion == 0) {
            if (fireCount == 0) return iceCount;
            fireCount--;
        } else {
            if (iceCount == 0) return fireCount;
            iceCount--;
        }
    }
    return 0;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static int countUnluckyApprentices(int[] apprentices, int[] potions) {
    int fireCount = 0;
    int iceCount = 0;

    for (int app : apprentices) {
        if (app == 0) fireCount++;
        else iceCount++;
    }

    for (int potion : potions) {
        if (potion == 0) {
            if (fireCount == 0) return iceCount;
            fireCount--;
        } else {
            if (iceCount == 0) return fireCount;
            iceCount--;
        }
    }
    return 0;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

int countUnluckyApprentices(int* apprentices, int apprenticesSize, int* potions, int potionsSize) {
    int fireCount = 0;
    int iceCount = 0;

    for (int i = 0; i < apprenticesSize; i++) {
        if (apprentices[i] == 0) fireCount++;
        else iceCount++;
    }

    for (int i = 0; i < potionsSize; i++) {
        if (potions[i] == 0) {
            if (fireCount == 0) return iceCount;
            fireCount--;
        } else {
            if (iceCount == 0) return fireCount;
            iceCount--;
        }
    }
    return 0;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function countUnluckyApprentices(apprentices, potions) {
    let fireCount = 0;
    let iceCount = 0;

    for (let app of apprentices) {
        if (app === 0) fireCount++;
        else iceCount++;
    }

    for (let potion of potions) {
        if (potion === 0) {
            if (fireCount === 0) return iceCount;
            fireCount--;
        } else {
            if (iceCount === 0) return fireCount;
            iceCount--;
        }
    }
    return 0;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def countUnluckyApprentices(apprentices: list, potions: list) -> int:
    fire_count = 0
    ice_count = 0

    for app in apprentices:
        if app == 0:
            fire_count += 1
        else:
            ice_count += 1

    for potion in potions:
        if potion == 0:
            if fire_count == 0:
                return ice_count
            fire_count -= 1
        else:
            if ice_count == 0:
                return fire_count
            ice_count -= 1
            
    return 0

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  