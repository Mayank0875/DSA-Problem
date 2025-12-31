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
        
        vector<int> nums(n);
        for (int i = 0; i < n; ++i) {
            cin >> nums[i];
        }
        
        int k;
        cin >> k;
        
        vector<int> result = getAverages(nums, k);
        
        for (size_t i = 0; i < result.size(); ++i) {
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
            
            int[] nums = new int[n];
            for (int i = 0; i < n; i++) {
                nums[i] = sc.nextInt();
            }

            int k = sc.nextInt();

            int[] result = getAverages(nums, k);

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
        if (scanf("%d", &n) != 1) return 0;

        int* nums = (int*)malloc(sizeof(int) * n);
        for (int i = 0; i < n; i++) {
            scanf("%d", &nums[i]);
        }

        int k;
        scanf("%d", &k);

        int* result = getAverages(nums, n, k);

        for (int i = 0; i < n; i++) {
            printf("%d", result[i]);
            if (i + 1 < n) printf(" ");
        }
        printf("\n");

        free(nums);
        free(result);

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

    const t = parseInt(input[idx++]);
    for (let tc = 0; tc < t; tc++) {
        const n = parseInt(input[idx++]);
        const nums = [];

        for (let i = 0; i < n; i++) {
            nums.push(parseInt(input[idx++]));
        }

        const k = parseInt(input[idx++]);

        const result = getAverages(nums, k);

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
        nums = list(map(int, input().split()))
        k = int(input())

        result = getAverages(nums, k)

        print(" ".join(map(str, result)))

        # evaluation completed

if __name__ == "__main__":
    main()
