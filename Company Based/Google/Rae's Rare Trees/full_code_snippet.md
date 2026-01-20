## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here


int main() {
    int t;
    cin >> t;

    while (t--) {
        int n;
        cin >> n;
        vector<int> p(n);
        for (int i = 0; i < n; ++i) {
            cin >> p[i];
        }
        if (solve(n, p)) {
            cout << "True" << endl;
        } else {
            cout << "False" << endl;
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
            int[] p = new int[n];

            for (int i = 0; i < n; i++) {
                p[i] = sc.nextInt();
            }

            if (solve(n, p)) {
                System.out.println("True");
            } else {
                System.out.println("False");
            }
            // evaluation completed
        }
        sc.close();
    }
}


## C

#include <stdio.h>
#include <stdbool.h>

// user code comes here

int main() {
    int t;
    scanf("%d", &t);

    while (t--) {
        int n;
        scanf("%d", &n);

        int p[n];
        for (int i = 0; i < n; i++) {
            scanf("%d", &p[i]);
        }

        if (solve(n, p)) {
            printf("True\n");
        } else {
            printf("False\n");
        }
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
        const p = [];

        for (let i = 0; i < n; i++) {
            p.push(Number(input[idx++]));
        }

        console.log(solve(n, p) ? "True" : "False");
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
        n = int(input())
        p = list(map(int, input().split()))

        print("True" if solve(n, p) else "False")
        # evaluation completed

if __name__ == "__main__":
    main()
