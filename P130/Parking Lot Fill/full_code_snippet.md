## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here


int main() {
    int t;
    cin >> t;

    while (t--) {
        int n;
        if (cin >> n) {
            vector<int> flips(n);
            for (int i = 0; i < n; i++) {
                cin >> flips[i];
            }
            cout << countAligned(flips) << endl;
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
            int[] flips = new int[n];

            for (int i = 0; i < n; i++) {
                flips[i] = sc.nextInt();
            }

            System.out.println(countAligned(flips));
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
        int n;
        scanf("%d", &n);

        int flips[n];
        for (int i = 0; i < n; i++) {
            scanf("%d", &flips[i]);
        }

        printf("%d\n", countAligned(flips, n));
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
        const flips = [];

        for (let i = 0; i < n; i++) {
            flips.push(Number(input[idx++]));
        }

        console.log(countAligned(flips));
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
        flips = list(map(int, input().split()))
        print(countAligned(flips))
        # evaluation completed

if __name__ == "__main__":
    main()
