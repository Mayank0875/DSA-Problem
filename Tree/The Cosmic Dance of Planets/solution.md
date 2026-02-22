## CPP

### SOLUTION

long long power(long long base, long long exp) {
    long long res = 1;
    base %= 1000000007;
    while (exp > 0) {
        if (exp % 2 == 1) res = (res * base) % 1000000007;
        base = (base * base) % 1000000007;
        exp /= 2;
    }
    return res;
}

int solve(int n, vector<int>& p) {
    vector<bool> vis(n, false);
    map<int, int> max_prime_power;
    vector<int> spf(n + 1);
    iota(spf.begin(), spf.end(), 0);
    for (int i = 2; i * i <= n; i++) {
        if (spf[i] == i) {
            for (int j = i * i; j <= n; j += i)
                if (spf[j] == j) spf[j] = i;
        }
    }

    for (int i = 0; i < n; i++) {
        if (!vis[i]) {
            int curr = i;
            int count = 0;
            while (!vis[curr]) {
                vis[curr] = true;
                curr = p[curr] - 1;
                count++;
            }
            
            int temp = count;
            while (temp > 1) {
                int pr = spf[temp];
                int cnt = 0;
                while (temp % pr == 0) {
                    temp /= pr;
                    cnt++;
                }
                max_prime_power[pr] = max(max_prime_power[pr], cnt);
            }
        }
    }

    long long ans = 1;
    for (auto const& [val, pwr] : max_prime_power) {
        ans = (ans * power(val, pwr)) % 1000000007;
    }
    return (int)ans;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION


private static long power(long base, long exp) {
    long res = 1;
    long mod = 1000000007;
    base %= mod;
    while (exp > 0) {
        if (exp % 2 == 1) res = (res * base) % mod;
        base = (base * base) % mod;
        exp /= 2;
    }
    return res;
}

public static int solve(int n, int[] p) {
    boolean[] vis = new boolean[n];
    Map<Integer, Integer> maxPrimePower = new HashMap<>();
    int[] spf = new int[n + 1];
    for (int i = 0; i <= n; i++) spf[i] = i;
    for (int i = 2; i * i <= n; i++) {
        if (spf[i] == i) {
            for (int j = i * i; j <= n; j += i)
                if (spf[j] == j) spf[j] = i;
        }
    }

    for (int i = 0; i < n; i++) {
        if (!vis[i]) {
            int curr = i;
            int count = 0;
            while (!vis[curr]) {
                vis[curr] = true;
                curr = p[curr] - 1;
                count++;
            }
            int temp = count;
            while (temp > 1) {
                int pr = spf[temp];
                int cnt = 0;
                while (temp % pr == 0) {
                    temp /= pr;
                    cnt++;
                }
                maxPrimePower.put(pr, Math.max(maxPrimePower.getOrDefault(pr, 0), cnt));
            }
        }
    }

    long ans = 1;
    long mod = 1000000007;
    for (Map.Entry<Integer, Integer> entry : maxPrimePower.entrySet()) {
        ans = (ans * power(entry.getKey(), entry.getValue())) % mod;
    }
    return (int) ans;
}


### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## JAVASCRIPT

### SOLUTION

function power(base, exp) {
    let res = 1n;
    let b = BigInt(base);
    let e = BigInt(exp);
    let mod = 1000000007n;
    while (e > 0n) {
        if (e % 2n === 1n) res = (res * b) % mod;
        b = (b * b) % mod;
        e = e / 2n;
    }
    return res;
}

function solve(n, p) {
    let vis = new Uint8Array(n);
    let spf = new Int32Array(n + 1);
    let maxPwr = new Map();
    for (let i = 0; i <= n; i++) spf[i] = i;
    for (let i = 2; i * i <= n; i++) {
        if (spf[i] === i) {
            for (let j = i * i; j <= n; j += i)
                if (spf[j] === j) spf[j] = i;
        }
    }

    for (let i = 0; i < n; i++) {
        if (!vis[i]) {
            let curr = i;
            let count = 0;
            while (!vis[curr]) {
                vis[curr] = 1;
                curr = p[curr] - 1;
                count++;
            }
            let temp = count;
            while (temp > 1) {
                let pr = spf[temp];
                let cnt = 0;
                while (temp % pr === 0) {
                    temp /= pr;
                    cnt++;
                }
                maxPwr.set(pr, Math.max(maxPwr.get(pr) || 0, cnt));
            }
        }
    }

    let ans = 1n;
    let mod = 1000000007n;
    for (let [val, pwr] of maxPwr) {
        ans = (ans * this.power(val, pwr)) % mod;
    }
    return Number(ans);
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  



## PYTHON

### SOLUTION

def solve(self, n: int, p: list) -> int:
    vis = [False] * n
    max_pwr = {}
    spf = list(range(n + 1))
    for i in range(2, int(n**0.5) + 1):
        if spf[i] == i:
            for j in range(i*i, n + 1, i):
                if spf[j] == j:
                    spf[j] = i
    
    for i in range(n):
        if not vis[i]:
            curr = i
            count = 0
            while not vis[curr]:
                vis[curr] = True
                curr = p[curr] - 1
                count += 1
            
            temp = count
            while temp > 1:
                pr = spf[temp]
                cnt = 0
                while temp % pr == 0:
                    temp //= pr
                    cnt += 1
                max_pwr[pr] = max(max_pwr.get(pr, 0), cnt)
    
    ans = 1
    MOD = 10**9 + 7
    for val, pwr in max_pwr.items():
        ans = (ans * pow(val, pwr, MOD)) % MOD
    return ans

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  