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
        
        vector<int> platforms(n);
        for (int i = 0; i < n; i++) {
            cin >> platforms[i];
        }
        
        if (canReachEnd(platforms)) {
            cout << "true" << endl;
        } else {
            cout << "false" << endl;
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
            int[] platforms = new int[n];

            for (int i = 0; i < n; i++) {
                platforms[i] = sc.nextInt();
            }

            if (canReachEnd(platforms)) {
                System.out.println("true");
            } else {
                System.out.println("false");
            }

            // evaluation completed
        }
        sc.close();
    }
}


## C

#include <stdio.h>
#include <stdlib.h>
#include <stdbool.h>

// user code comes here

int main() {
    int t;
    scanf("%d", &t);

    while (t--) {
        int n;
        if (scanf("%d", &n) != 1) return 0;

        int* platforms = (int*)malloc(n * sizeof(int));
        for (int i = 0; i < n; i++) {
            scanf("%d", &platforms[i]);
        }

        if (canReachEnd(platforms, n)) {
            printf("true\n");
        } else {
            printf("false\n");
        }

        free(platforms);

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
        const platforms = new Array(n);

        for (let i = 0; i < n; i++) {
            platforms[i] = Number(input[idx++]);
        }

        if (canReachEnd(platforms)) {
            console.log("true");
        } else {
            console.log("false");
        }

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
        platforms = list(map(int, input().split()))

        if canReachEnd(platforms):
            print("true")
        else:
            print("false")

        # evaluation completed

if __name__ == "__main__":
    main()
