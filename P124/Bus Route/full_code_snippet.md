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
            vector<int> nums(n);
            for (int i = 0; i < n; i++) {
                cin >> nums[i];
            }
            cout << (checkSubarraySum(nums, k) ? "true" : "false") << endl;
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
            int n = scanner.nextInt();
            int k = scanner.nextInt();
            int[] nums = new int[n];
            for (int i = 0; i < n; i++) {
                nums[i] = scanner.nextInt();
            }
            System.out.println(checkSubarraySum(nums, k) ? "true" : "false");
            // evaluation completed
        }
        sc.close();
    }
}

## C

#include <stdio.h>
#include <stdbool.h>
#include <stdlib.h>
#include <math.h>


// user code comes here


int main() {
    int t;
    scanf("%d", &t);
    while (t--) {
        int* nums = (int*)malloc(n * sizeof(int));
        for (int i = 0; i < n; i++) {
            scanf("%d", &nums[i]);
        }
        
        if (checkSubarraySum(nums, n, k)) {
            printf("true\n");
        } else {
            printf("false\n");
        }
        
        free(nums);
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
        const k = parseInt(input[idx++]);
        const nums = [];
        for (let i = 0; i < n; i++) {
            nums.push(parseInt(input[idx++]));
        }

        console.log(checkSubarraySum(nums, k) ? "true" : "false");
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
        n, k = map(int, input().split())
        nums = list(map(int, input().split()))
        print("true" if checkSubarraySum(nums, k) else "false")
        # evaluation completed

if __name__ == "__main__":
    main()