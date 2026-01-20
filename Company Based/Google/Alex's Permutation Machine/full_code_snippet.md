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
        vector<int> nums(n);
        for (int i = 0; i < n; ++i) cin >> nums[i];
        vector<int> ans = buildArray(nums);
        for (int i = 0; i < n; ++i) cout << ans[i] << (i == n - 1 ? "" : " ");
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

            int[] ans = buildArray(nums);
            for (int i = 0; i < n; i++) {
                System.out.print(ans[i]);
                if (i + 1 < n) System.out.print(" ");
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

        int nums[n];
        for (int i = 0; i < n; i++) {
            scanf("%d", &nums[i]);
        }

        int returnSize;
        int* ans = buildArray(nums, n, &returnSize);

        for (int i = 0; i < returnSize; i++) {
            printf("%d", ans[i]);
            if (i + 1 < returnSize) printf(" ");
        }
        printf("\n");
        // evaluation completed

        free(ans);
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
        const nums = [];

        for (let i = 0; i < n; i++) {
            nums.push(Number(input[idx++]));
        }

        const ans = buildArray(nums);
        console.log(ans.join(" "));
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
        nums = list(map(int, input().split()))

        ans = buildArray(nums)
        print(" ".join(map(str, ans)))
        # evaluation completed

if __name__ == "__main__":
    main()
