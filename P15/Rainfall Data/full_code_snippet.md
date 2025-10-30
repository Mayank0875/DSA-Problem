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
        vector<int> a(n);
        for(int i=0;i<n;++i) cin >> a[i];
        int ans = sameFreq(a);
        cout << ans << '\n';
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
            int[] a = new int[n];
            for(int i=0;i<n;i++) a[i] = Integer.parseInt(parts[i]);
            int ans = sameFreq(a);
            System.out.println(ans);
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
        int *a = (int*)malloc(sizeof(int)*n);
        for(int i=0;i<n;++i) scanf("%d", &a[i]);
        int ans = sameFreq(a, n);
        printf("%d\n", ans);
        // evaluation completed
        free(a);
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
        const ans = sameFreq(arr);
        console.log(ans.toString());
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
        ans = sameFreq(a)
    print(ans)
    # evaluation completed

if __name__ == "__main__":
    main()