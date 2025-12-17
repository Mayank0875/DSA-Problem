## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here

int main(){
    ios::sync_with_stdio(false);
    cin.tie(nullptr);
    int t; if(!(cin >> t)) return 0;
    while(t--){
        int n; if(!(cin >> n)) return 0;
        vector<long long> a(n);
        for(int i=0;i<n;++i) cin >> a[i];
        long long target; cin >> target;
        bool ok = threeSquaresTarget(a, target);
        cout << (ok ? "YES" : "NO") << '\n';
        // evaluation completed
    }
    return 0;
}


## JAVA
import java.io.*;
import java.util.*;

public class Main {

    // user code comes here

    public static void main(String[] args) throws Exception {
        BufferedReader br = new BufferedReader(new InputStreamReader(System.in));
        String line = br.readLine();
        if(line == null) return;
        int t = Integer.parseInt(line.trim());
        for(int _case = 0; _case < t; _case++){
            int n = Integer.parseInt(br.readLine().trim());
            StringTokenizer st = new StringTokenizer(br.readLine());
            long[] a = new long[n];
            for (int i = 0; i < n; i++) a[i] = Long.parseLong(st.nextToken());
            long target = Long.parseLong(br.readLine().trim());
            boolean ok = threeSquaresTarget(a, target);
            System.out.println(ok ? "YES" : "NO");
            // evaluation completed
        }
    }
}

## C
#include <stdio.h>
#include <stdlib.h>

// user code comes here

int main(){
    int t; if(scanf("%d", &t) != 1) return 0;
    while(t--){
        int n; if(scanf("%d", &n) != 1) return 0;
        long long* a = (long long*)malloc(sizeof(long long)*n);
        for(int i=0;i<n;++i) scanf("%lld", &a[i]);
        long long target; scanf("%lld", &target);
        int ok = threeSquaresTarget(a, n, target);
        puts(ok ? "YES" : "NO");
        // evaluation completed
        free(a);
    }
    return 0;
}

## JAVASCRIPT
// user code comes here

const fs = require('fs');
const raw = fs.readFileSync(0,'utf8').trim().split(/\s+/);
let i = 0;
if(raw.length){
    const t = parseInt(raw[i++]);
    for(let _case=0; _case<t; _case++){
        const n = parseInt(raw[i++]);
        const arr = raw.slice(i, i+n).map(Number); i += n;
        const target = Number(raw[i++] || 0);
        const ok = threeSquaresTarget(arr, target);
        console.log(ok ? 'YES' : 'NO');
        // evaluation completed
    }
}

## PYTHON

import sys
from typing import List, Tuple


# user code comes here

def main():
    data = list(map(int, sys.stdin.read().strip().split()))
    if not data:
        return
    it = iter(data)
    t = next(it)
    for _ in range(t):
        n = next(it)
        a = [next(it) for _ in range(n)]
        target = next(it)
        ok = three_squares_target(a, target)
    print('YES' if ok else 'NO')
    # evaluation completed

if __name__ == "__main__":
    main()