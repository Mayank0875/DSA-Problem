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
        
        vector<vector<int>> pairs(n, vector<int>(2));
        for(int i = 0; i < n; ++i) {
            cin >> pairs[i][0] >> pairs[i][1];
        }

        cout << findLongestChain(pairs) << endl;
        
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
            int[][] pairs = new int[n][2];

            for (int i = 0; i < n; i++) {
                pairs[i][0] = sc.nextInt();
                pairs[i][1] = sc.nextInt();
            }

            System.out.println(findLongestChain(pairs));

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

        int** pairs = (int**)malloc(n * sizeof(int*));
        for (int i = 0; i < n; i++) {
            pairs[i] = (int*)malloc(2 * sizeof(int));
            scanf("%d %d", &pairs[i][0], &pairs[i][1]);
        }

        printf("%d\n", findLongestChain(pairs, n));

        for (int i = 0; i < n; i++) {
            free(pairs[i]);
        }
        free(pairs);

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
        const pairs = new Array(n);

        for (let i = 0; i < n; i++) {
            const a = Number(input[idx++]);
            const b = Number(input[idx++]);
            pairs[i] = [a, b];
        }

        console.log(findLongestChain(pairs));

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
        pairs = []

        for _ in range(n):
            a, b = map(int, input().split())
            pairs.append([a, b])

        print(findLongestChain(pairs))

        # evaluation completed

if __name__ == "__main__":
    main()
