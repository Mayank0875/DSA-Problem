## CPP

### SOLUTION

long long MOD = 1000000007;

std::tuple<int, int, int> extended_euclid_algo(int a, int b) {
    if (a == 0) return std::make_tuple(0, 1, b);
    int x1, y1, g;
    std::tie(x1, y1, g) = extended_euclid_algo(b % a, a);
    return std::make_tuple((y1 - (b / a) * x1), x1, g);
}

int modular_inverse(int a, int m) {
    int x, y, g;
    std::tie(x, y, g) = extended_euclid_algo(a, m);
    return (x % m + m) % m;
}

int countDistinctStrings(string str) {
    int n = str.size();
    std::vector<long long> fact(n + 1);
    fact[0] = 1;
    for (int i = 1; i <= n; ++i) {
        fact[i] = (fact[i - 1] * i) % MOD;
    }

    std::map<char, int> fre;
    for (char ch : str) {
        fre[ch]++;
    }

    long long res = fact[n];
    for (auto const& [key, val] : fre) {
        long long denominator = fact[val];
        long long inverse = modular_inverse(denominator, MOD);
        res = (res * inverse) % MOD;
    }
    return (int)res;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

static long MOD = 1000000007L;

public static long[] extended_euclid_algo(long a, long b) {
    if (a == 0) return new long[]{0, 1, b};
    long[] res = extended_euclid_algo(b % a, a);
    long x1 = res[0];
    long y1 = res[1];
    long g = res[2];
    return new long[]{y1 - (b / a) * x1, x1, g};
}

public static long modular_inverse(long a, long m) {
    long[] res = extended_euclid_algo(a, m);
    return (res[0] % m + m) % m;
}

public static int countDistinctStrings(String str) {
    int n = str.length();
    long[] fact = new long[n + 1];
    fact[0] = 1;
    for (int i = 1; i <= n; ++i) {
        fact[i] = (fact[i - 1] * i) % MOD;
    }

    java.util.Map<Character, Integer> fre = new java.util.HashMap<>();
    for (char ch : str.toCharArray()) {
        fre.put(ch, fre.getOrDefault(ch, 0) + 1);
    }

    long res = fact[n];
    for (int val : fre.values()) {
        long denominator = fact[val];
        long inverse = modular_inverse(denominator, MOD);
        res = (res * inverse) % MOD;
    }
    return (int)res;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  

