## CPP

### SOLUTION

long long trapRainWater(vector<int>& height) {
    int n = height.size();
    if (n <= 2) {
        return 0;
    }

    long long totalWater = 0;
    int left = 0;
    int right = n - 1;
    int maxLeft = 0;
    int maxRight = 0;

    while (left < right) {
        if (height[left] < height[right]) {
            if (height[left] >= maxLeft) {
                maxLeft = height[left];
            } else {
                totalWater += maxLeft - height[left];
            }
            left++;
        } else {
            if (height[right] >= maxRight) {
                maxRight = height[right];
            } else {
                totalWater += maxRight - height[right];
            }
            right--;
        }
    }
    return totalWater;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static long trapRainWater(List<Integer> height) {
    int n = height.size();
    if (n <= 2) return 0;

    long totalWater = 0;
    int left = 0, right = n - 1;
    int maxLeft = 0, maxRight = 0;

    while (left < right) {
        if (height.get(left) < height.get(right)) {
            if (height.get(left) >= maxLeft)
                maxLeft = height.get(left);
            else
                totalWater += maxLeft - height.get(left);
            left++;
        } else {
            if (height.get(right) >= maxRight)
                maxRight = height.get(right);
            else
                totalWater += maxRight - height.get(right);
            right--;
        }
    }
    return totalWater;
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## C

### SOLUTION

long long trapRainWater(int* height, int n) {
    if (n <= 2) return 0;

    long long totalWater = 0;
    int left = 0, right = n - 1;
    int maxLeft = 0, maxRight = 0;

    while (left < right) {
        if (height[left] < height[right]) {
            if (height[left] >= maxLeft)
                maxLeft = height[left];
            else
                totalWater += (long long)(maxLeft - height[left]);
            left++;
        } else {
            if (height[right] >= maxRight)
                maxRight = height[right];
            else
                totalWater += (long long)(maxRight - height[right]);
            right--;
        }
    }
    return totalWater;
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function trapRainWater(height) {
    const n = height.length;
    if (n <= 2) return 0;

    let totalWater = 0;
    let left = 0, right = n - 1;
    let maxLeft = 0, maxRight = 0;

    while (left < right) {
        if (height[left] < height[right]) {
            if (height[left] >= maxLeft)
                maxLeft = height[left];
            else
                totalWater += maxLeft - height[left];
            left++;
        } else {
            if (height[right] >= maxRight)
                maxRight = height[right];
            else
                totalWater += maxRight - height[right];
            right--;
        }
    }
    return totalWater;
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def trapRainWater(height):
    n = len(height)
    if n <= 2:
        return 0

    total_water = 0
    left, right = 0, n - 1
    max_left, max_right = 0, 0

    while left < right:
        if height[left] < height[right]:
            if height[left] >= max_left:
                max_left = height[left]
            else:
                total_water += max_left - height[left]
            left += 1
        else:
            if height[right] >= max_right:
                max_right = height[right]
            else:
                total_water += max_right - height[right]
            right -= 1

    return total_water


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  