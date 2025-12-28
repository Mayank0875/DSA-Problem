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
        
        vector<int> rungs(n);
        for (int i = 0; i < n; i++) {
            cin >> rungs[i];
        }
        
        cout << longestConsecutiveRun(rungs) << endl;
            
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
            int[] rungs = new int[n];

            for (int i = 0; i < n; i++) {
                rungs[i] = sc.nextInt();
            }

            System.out.println(longestConsecutiveRun(rungs));

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

        int* rungs = (int*)malloc(n * sizeof(int));
        for (int i = 0; i < n; i++) {
            scanf("%d", &rungs[i]);
        }

        printf("%d\n", longestConsecutiveRun(rungs, n));

        free(rungs);

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
        const rungs = new Array(n);

        for (let i = 0; i < n; i++) {
            rungs[i] = Number(input[idx++]);
        }

        console.log(longestConsecutiveRun(rungs));

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
        rungs = list(map(int, input().split()))

        print(longestConsecutiveRun(rungs))

        # evaluation completed

if __name__ == "__main__":
    main()
