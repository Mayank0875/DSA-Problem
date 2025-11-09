## CPP

### SOLUTION

int countBalancedTriplets(vector<int>& ratings) {
    sort(ratings.begin(), ratings.end());
    int n = ratings.size();
    int count = 0;

    for (int i = 0; i < n - 2; ++i) {
        if (i > 0 && ratings[i] == ratings[i - 1]) {
            continue;
        }
        int left = i + 1;
        int right = n - 1;
        int target = -ratings[i];

        while (left < right) {
            int sum = ratings[left] + ratings[right];

            if (sum == target) {
                count++;
                while (left < right && ratings[left] == ratings[left + 1]) {
                    left++;
                }
                while (left < right && ratings[right] == ratings[right - 1]) {
                    right--;
                }
                left++;
                right--;
            } else if (sum < target) {
                left++;
            } else {
                right--;
            }
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

public static int countBalancedTriplets(int[] ratings) {
    Arrays.sort(ratings);
    int n = ratings.length;
    int count = 0;

    for (int i = 0; i < n - 2; i++) {
        if (i > 0 && ratings[i] == ratings[i - 1]) continue;
        int left = i + 1, right = n - 1;
        int target = -ratings[i];

        while (left < right) {
            int sum = ratings[left] + ratings[right];
            if (sum == target) {
                count++;
                while (left < right && ratings[left] == ratings[left + 1]) left++;
                while (left < right && ratings[right] == ratings[right - 1]) right--;
                left++; right--;
            } else if (sum < target) left++;
            else right--;
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

int cmp(const void *a, const void *b) {
    return (*(int*)a - *(int*)b);
}

int countBalancedTriplets(int ratings[], int n) {
    qsort(ratings, n, sizeof(int), cmp);
    int count = 0;

    for (int i = 0; i < n - 2; i++) {
        if (i > 0 && ratings[i] == ratings[i - 1]) continue;
        int left = i + 1, right = n - 1;
        int target = -ratings[i];

        while (left < right) {
            int sum = ratings[left] + ratings[right];
            if (sum == target) {
                count++;
                while (left < right && ratings[left] == ratings[left + 1]) left++;
                while (left < right && ratings[right] == ratings[right - 1]) right--;
                left++; right--;
            } else if (sum < target) left++;
            else right--;
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

function countBalancedTriplets(ratings) {
    ratings.sort((a, b) => a - b);
    const n = ratings.length;
    let count = 0;

    for (let i = 0; i < n - 2; i++) {
        if (i > 0 && ratings[i] === ratings[i - 1]) continue;
        let left = i + 1, right = n - 1;
        const target = -ratings[i];

        while (left < right) {
            const sum = ratings[left] + ratings[right];
            if (sum === target) {
                count++;
                while (left < right && ratings[left] === ratings[left + 1]) left++;
                while (left < right && ratings[right] === ratings[right - 1]) right--;
                left++;
                right--;
            } else if (sum < target) left++;
            else right--;
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

def countBalancedTriplets(ratings):
    ratings.sort()
    n = len(ratings)
    count = 0

    for i in range(n - 2):
        if i > 0 and ratings[i] == ratings[i - 1]:
            continue
        left, right = i + 1, n - 1
        target = -ratings[i]

        while left < right:
            s = ratings[left] + ratings[right]
            if s == target:
                count += 1
                while left < right and ratings[left] == ratings[left + 1]:
                    left += 1
                while left < right and ratings[right] == ratings[right - 1]:
                    right -= 1
                left += 1
                right -= 1
            elif s < target:
                left += 1
            else:
                right -= 1

    return count



### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  