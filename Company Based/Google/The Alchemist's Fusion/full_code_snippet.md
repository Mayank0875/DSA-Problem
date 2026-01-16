## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here


int main() {
    int t;
    cin >> t;

    while (t--) {
        int n, k;
        if (cin >> n >> k) {
            vector<int> a(n);
            for (int i = 0; i < n; i++) {
                cin >> a[i];
            }
            cout << countPerfectPairs(n, k, a) << endl;
        }
            
        // evaluation completed
    }
    return 0;
}

## JAVA

import java.util.*;

public class Main {

    // user code comes here

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int t = sc.nextInt();

        while (t-- > 0) {
            int n = sc.nextInt();
            int k = sc.nextInt();

            int[] a = new int[n];
            for (int i = 0; i < n; i++) {
                a[i] = sc.nextInt();
            }

            System.out.println(countPerfectPairs(n, k, a));
            // evaluation completed
        }
        sc.close();
    }
}


## C

#include <stdio.h>

// user code comes here

int main() {
    int t;
    scanf("%d", &t);

    while (t--) {
        int n, k;
        scanf("%d %d", &n, &k);

        int a[n];
        for (int i = 0; i < n; i++) {
            scanf("%d", &a[i]);
        }

        printf("%lld\n", countPerfectPairs(n, k, a));
        // evaluation completed
    }
    return 0;
}


## JAVASCRIPT

// user code comes here

function main() {
    const fs = require("fs");
    const input = fs.readFileSync(0, "utf-8").trim().split(/\s+/);
    let idx = 0;

    const t = Number(input[idx++]);

    for (let tc = 0; tc < t; tc++) {
        const n = Number(input[idx++]);
        const k = Number(input[idx++]);

        const a = [];
        for (let i = 0; i < n; i++) {
            a.push(Number(input[idx++]));
        }

        console.log(countPerfectPairs(n, k, a));
        // evaluation completed
    }
}

main();


## PYTHON

import math
from typing import List

# user code comes here

def main():
    t = int(input())
    for _ in range(t):
        n, k = map(int, input().split())
        a = list(map(int, input().split()))

        print(countPerfectPairs(n, k, a))
        # evaluation completed

if __name__ == "__main__":
    main()
