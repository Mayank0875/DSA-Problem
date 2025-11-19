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
        vector<long long> ans = Numbers(a);
        for(size_t i=0;i<ans.size();++i){ if(i) cout << ' '; cout << ans[i]; }
        cout << '\n';
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
        if (line == null) return;
        int t = Integer.parseInt(line.trim());
        for(int _case = 0; _case < t; _case++){
            int n = Integer.parseInt(br.readLine().trim());
            String[] parts = br.readLine().trim().split(" ");
            long[] a = new long[n];
            for(int i=0;i<n;i++) a[i] = Long.parseLong(parts[i]);
            long[] ans = Numbers(a);
            StringBuilder sb = new StringBuilder();
            for(int i=0;i<ans.length;i++){ if(i>0) sb.append(' '); sb.append(ans[i]); }
            System.out.println(sb.toString());
            // evaluation completed
        }
    }
}

## C
#include <stdio.h>
#include <stdlib.h>
#include <string.h>

// user code comes here

int main(){
    int t; if(scanf("%d", &t) != 1) return 0;
    while(t--){
        int n; if(scanf("%d", &n) != 1) return 0;
        long long *a = (long long*)malloc(sizeof(long long)*n);
        for(int i=0;i<n;++i) scanf("%lld", &a[i]);
        long long* out=NULL; int m=0;
        Numbers(a, n, &out, &m);
        for(int i=0;i<m;i++){ if(i) printf(" "); printf("%lld", out[i]); }
        printf("\n");
        // evaluation completed
        free(out); free(a);
    }
    return 0;
}

## JAVASCRIPT
// user code comes here

const fs = require('fs');
const data = fs.readFileSync(0,'utf8').trim().split(/\s+/).map(Number);
let i = 0;
if (data.length) {
    const t = data[i++];
    for (let _case = 0; _case < t; _case++){
        const n = data[i++];
        const arr = data.slice(i, i+n); i += n;
        const ans = Numbers(arr);
        console.log(ans.join(' '));
        // evaluation completed
    }
}

## PYTHON

import sys
from typing import List

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
        ans = Numbers(a)
    print(' '.join(map(str, ans)))
    # evaluation completed

if __name__ == "__main__":
    main()