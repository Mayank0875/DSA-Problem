## CPP

### SOLUTION

long long minFaultTolerantCost(int n, vector<int>& a, vector<int>& b) {
    long long ans = abs(a[0] - b[0]) + abs(a[n - 1] - b[n - 1]);
    ans = min(ans, (long long)abs(a[0] - b[n - 1]) + abs(a[n - 1] - b[0]));

    long long ma = 2e18, mb = 2e18, mc = 2e18, md = 2e18;

    for (int i = 0; i < n; i++) {
        ma = min(ma, (long long)abs(a[0] - b[i]));
        mb = min(mb, (long long)abs(a[n - 1] - b[i]));
        mc = min(mc, (long long)abs(b[0] - a[i]));
        md = min(md, (long long)abs(b[n - 1] - a[i]));
    }

    ans = min(ans, (long long)abs(a[0] - b[0]) + mb + md);
    ans = min(ans, (long long)abs(a[n - 1] - b[n - 1]) + ma + mc);
    ans = min(ans, ma + mc + mb + md);
    ans = min(ans, (long long)abs(a[0] - b[n - 1]) + mc + mb);
    ans = min(ans, (long long)abs(a[n - 1] - b[0]) + ma + md);

    return ans;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


## JAVA

### SOLUTION

public static long minFaultTolerantCost(int n, int[] a, int[] b) {
    long ans = Math.abs((long)a[0] - b[0]) + Math.abs((long)a[n - 1] - b[n - 1]);
    ans = Math.min(ans, Math.abs((long)a[0] - b[n - 1]) + Math.abs((long)a[n - 1] - b[0]));

    long ma = Long.MAX_VALUE, mb = Long.MAX_VALUE, mc = Long.MAX_VALUE, md = Long.MAX_VALUE;

    for (int i = 0; i < n; i++) {
        ma = Math.min(ma, Math.abs((long)a[0] - b[i]));
        mb = Math.min(mb, Math.abs((long)a[n - 1] - b[i]));
        mc = Math.min(mc, Math.abs((long)b[0] - a[i]));
        md = Math.min(md, Math.abs((long)b[n - 1] - a[i]));
    }

    ans = Math.min(ans, Math.abs((long)a[0] - b[0]) + mb + md);
    ans = Math.min(ans, Math.abs((long)a[n - 1] - b[n - 1]) + ma + mc);
    ans = Math.min(ans, ma + mc + mb + md);
    ans = Math.min(ans, Math.abs((long)a[0] - b[n - 1]) + mc + mb);
    ans = Math.min(ans, Math.abs((long)a[n - 1] - b[0]) + ma + md);

    return ans;
}

### METADATA

**TimeLimit**  
1000  

**MemoryLimit**  
512  


