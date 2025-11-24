## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here

int main() {
    int t;
    cin >> t;

    while (t--) {
        int n, m;
        cin >> n;
        vector<int> nums1(n);
        for (int i = 0; i < n; ++i) {
            cin >> nums1[i];
        }
        
        cin >> m;
        vector<int> nums2(m);
        for (int i = 0; i < m; ++i) {
            cin >> nums2[i];
        }
        
        cout << findLength(nums1, nums2) << endl;
        
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
            int[] nums1 = new int[n];
            for (int i = 0; i < n; i++) {
                nums1[i] = sc.nextInt();
            }

            int m = sc.nextInt();
            int[] nums2 = new int[m];
            for (int i = 0; i < m; i++) {
                nums2[i] = sc.nextInt();
            }

            System.out.println(findLength(nums1, nums2));
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
        int n, m;
        scanf("%d", &n);
        int* nums1 = (int*)malloc(n * sizeof(int));
        for (int i = 0; i < n; i++) {
            scanf("%d", &nums1[i]);
        }

        scanf("%d", &m);
        int* nums2 = (int*)malloc(m * sizeof(int));
        for (int i = 0; i < m; i++) {
            scanf("%d", &nums2[i]);
        }

        printf("%d\n", findLength(nums1, n, nums2, m));

        free(nums1);
        free(nums2);

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
        const nums1 = [];
        for (let i = 0; i < n; i++) {
            nums1.push(parseInt(input[idx++]));
        }

        const m = parseInt(input[idx++]);
        const nums2 = [];
        for (let i = 0; i < m; i++) {
            nums2.push(parseInt(input[idx++]));
        }

        console.log(findLength(nums1, nums2));
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
        nums1 = list(map(int, input().split()))

        m = int(input())
        nums2 = list(map(int, input().split()))

        print(findLength(nums1, nums2))
        # evaluation completed

if __name__ == "__main__":
    main()