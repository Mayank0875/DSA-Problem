## CPP

### SOLUTION

long long MinimumTime(int n, long long t, vector<int>& k) {
    long long low = 1;
    long long high = 1e18;
    long long ans = high;

    while (low <= high) {
        long long mid = low + (high - low) / 2;
        long long products_made = 0;
        bool overflow = false;
        for (int time_per_product : k) {
            if (time_per_product == 0) {
                 products_made = t;
                 overflow = true;
                 break;
            }
             long long current_machine_products = mid / time_per_product;
             if (products_made > t - current_machine_products) {
                  overflow = true;
                  break; 
             }
            products_made += current_machine_products;
             if (products_made >= t) {
                overflow = true; 
                break;
            }
        }

        if (overflow || products_made >= t) {
            ans = mid;
            high = mid - 1;
        } else {
            low = mid + 1;
        }
    }
    return ans;
}


### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## JAVA

### SOLUTION

public class Main {
    public static long MinimumTime(int n, long t, List<Integer> k) {
        long low = 1;
        long high = (long) 1e18;
        long ans = high;

        while (low <= high) {
            long mid = low + (high - low) / 2;
            long productsMade = 0;
            boolean overflow = false;

            for (int timePerProduct : k) {
                if (timePerProduct == 0) {
                    productsMade = t;
                    overflow = true;
                    break;
                }

                long currentMachineProducts = mid / timePerProduct;
                if (productsMade > t - currentMachineProducts) {
                    overflow = true;
                    break;
                }

                productsMade += currentMachineProducts;
                if (productsMade >= t) {
                    overflow = true;
                    break;
                }
            }

            if (overflow || productsMade >= t) {
                ans = mid;
                high = mid - 1;
            } else {
                low = mid + 1;
            }
        }

        return ans;
    }
}

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## C

### SOLUTION


long long MinimumTime(int n, long long t, int k[]) {
    long long low = 1;
    long long high = 1e18;
    long long ans = high;

    while (low <= high) {
        long long mid = low + (high - low) / 2;
        long long products_made = 0;
        bool overflow = false;

        for (int i = 0; i < n; i++) {
            int time_per_product = k[i];
            if (time_per_product == 0) {
                products_made = t;
                overflow = true;
                break;
            }

            long long current_machine_products = mid / time_per_product;
            if (products_made > t - current_machine_products) {
                overflow = true;
                break;
            }

            products_made += current_machine_products;
            if (products_made >= t) {
                overflow = true;
                break;
            }
        }

        if (overflow || products_made >= t) {
            ans = mid;
            high = mid - 1;
        } else {
            low = mid + 1;
        }
    }

    return ans;
}

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## JAVASCRIPT

### SOLUTION

function MinimumTime(n, t, k) {
    let low = 1n;
    let high = 10n ** 18n;
    let ans = high;

    while (low <= high) {
        let mid = low + (high - low) / 2n;
        let productsMade = 0n;
        let overflow = false;

        for (let timePerProduct of k) {
            if (timePerProduct === 0) {
                productsMade = BigInt(t);
                overflow = true;
                break;
            }

            let currentMachineProducts = mid / BigInt(timePerProduct);
            if (productsMade > BigInt(t) - currentMachineProducts) {
                overflow = true;
                break;
            }

            productsMade += currentMachineProducts;
            if (productsMade >= BigInt(t)) {
                overflow = true;
                break;
            }
        }

        if (overflow || productsMade >= BigInt(t)) {
            ans = mid;
            high = mid - 1n;
        } else {
            low = mid + 1n;
        }
    }

    return ans;
}

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256

## PYTHON

### SOLUTION

def MinimumTime(n: int, t: int, k: List[int]) -> int:
    low = 1
    high = 10**18
    ans = high

    while low <= high:
        mid = (low + high) // 2
        products_made = 0
        overflow = False

        for time_per_product in k:
            if time_per_product == 0:
                products_made = t
                overflow = True
                break

            current_machine_products = mid // time_per_product
            if products_made > t - current_machine_products:
                overflow = True
                break

            products_made += current_machine_products
            if products_made >= t:
                overflow = True
                break

        if overflow or products_made >= t:
            ans = mid
            high = mid - 1
        else:
            low = mid + 1

    return ans

### METADATA

**TimeLimit**
2000

**MemoryLimit**
256
