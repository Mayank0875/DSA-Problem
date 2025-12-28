## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here


int main() {
    int t;
    cin >> t;

    while (t--) {
        int n;
        if (!(cin >> n)) return 0;
        vector<int> canisters(n);
        for (int i = 0; i < n; i++) {
            cin >> canisters[i];
        }
        int result = maxValue(canisters);
        cout << result << endl;
        
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
            int[] canisters = new int[n];

            for (int i = 0; i < n; i++) {
                canisters[i] = sc.nextInt();
            }

            int result = maxValue(canisters);
            System.out.println(result);

            // evaluation completed
        }
        sc.close();
    }
}


## C

#include <stdio.h>
#include <stdlib.h>

// user code comes here

int main() {
    int t;
    scanf("%d", &t);

    while (t--) {
        int n;
        if (scanf("%d", &n) != 1) return 0;

        int* canisters = (int*)malloc(n * sizeof(int));
        for (int i = 0; i < n; i++) {
            scanf("%d", &canisters[i]);
        }

        int result = maxValue(canisters, n);
        printf("%d\n", result);

        free(canisters);

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
        const canisters = new Array(n);

        for (let i = 0; i < n; i++) {
            canisters[i] = Number(input[idx++]);
        }

        const result = maxValue(canisters);
        console.log(result);

        // evaluation completed
    }
}

main();


## PYTHON

import math
from typing import List
import collections

# user code comes here

def main():
    t = int(input())

    for _ in range(t):
        n = int(input())
        canisters = list(map(int, input().split()))

        result = maxValue(canisters)
        print(result)

        # evaluation completed

if __name__ == "__main__":
    main()
