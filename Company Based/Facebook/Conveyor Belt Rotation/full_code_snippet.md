## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here

int main() {
    int t;
    cin >> t;

    while (t--) {
        int n, k; 
        cin >> n >> k;
        vector<int> arr(n);
        for (int i = 0; i < n; ++i) cin >> arr[i];

        vector<int> res = rotateArray(arr, k);
        for (int i = 0; i < n; ++i) {
            cout << res[i] << ' ';
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
            int k = sc.nextInt();
            List<Integer> arr = new ArrayList<>();
            for (int i = 0; i < n; i++) {
                arr.add(sc.nextInt());
            }

            List<Integer> res = rotateArray(arr, k);
            for (int num : res) {
                System.out.print(num + " ");
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
        int n, k;
        scanf("%d %d", &n, &k);
        int arr[n];
        for (int i = 0; i < n; i++) {
            scanf("%d", &arr[i]);
        }

        int* res = rotateArray(arr, n, k);
        for (int i = 0; i < n; i++) {
            printf("%d ", res[i]);
        }
        printf("\n");
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
        const arr = [];
        for (let i = 0; i < n; i++) {
            arr.push(parseInt(input[idx++]));
        }

        const res = rotateArray(arr, k);
        console.log(res.join(" "));
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
        arr = list(map(int, input().split()))
        res = rotateArray(arr, k)
        print(" ".join(map(str, res)))
        # evaluation completed

if __name__ == "__main__":
    main()