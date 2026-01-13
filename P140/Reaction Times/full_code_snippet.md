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
        
        vector<int> arr(n);
        for(int i = 0; i < n; ++i) {
            cin >> arr[i];
        }
        
        vector<int> result = findKiteRanks(arr);
        
        for(size_t i = 0; i < result.size(); ++i) {
            cout << result[i] << (i == result.size() - 1 ? "" : " ");
        }
        cout << endl;
            
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
            int[] arr = new int[n];

            for (int i = 0; i < n; i++) {
                arr[i] = sc.nextInt();
            }

            int[] result = findKiteRanks(arr);

            for (int i = 0; i < result.length; i++) {
                System.out.print(result[i]);
                if (i + 1 < result.length) System.out.print(" ");
            }
            System.out.println();
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
        scanf("%d", &n);

        int arr[n];
        for (int i = 0; i < n; i++) {
            scanf("%d", &arr[i]);
        }

        int returnSize;
        int* result = findKiteRanks(arr, n, &returnSize);

        for (int i = 0; i < returnSize; i++) {
            printf("%d", result[i]);
            if (i + 1 < returnSize) printf(" ");
        }
        printf("\n");
        // evaluation completed

        free(result);
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
        const arr = [];

        for (let i = 0; i < n; i++) {
            arr.push(Number(input[idx++]));
        }

        const result = findKiteRanks(arr);
        console.log(result.join(" "));
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
        arr = list(map(int, input().split()))
        result = findKiteRanks(arr)
        print(" ".join(map(str, result)))
        # evaluation completed

if __name__ == "__main__":
    main()
