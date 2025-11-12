## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here


int main() {
    int t;
    cin >> t;

    while (t--) {
        int n, original; cin >> n >> original;
        vector<int> arr(n);
        for(int i = 0; i < n; ++i) cin >> arr[i];
        cout << findFinalValue(arr, original) << "\n";
        
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
            int original = sc.nextInt();
            List<Integer> arr = new ArrayList<>();
            for (int i = 0; i < n; i++) {
                arr.add(sc.nextInt());
            }
            System.out.println(findFinalValue(arr, original));
            // evaluation completed
        }
        sc.close();
    }
}

## C

#include <stdio.h>
#include <stdbool.h>
#include <stdlib.h>

// user code comes here

int main() {
    int t;
    scanf("%d", &t);
    while (t--) {
        int n, original;
        scanf("%d %d", &n, &original);
        int arr[n];
        for (int i = 0; i < n; i++) {
            scanf("%d", &arr[i]);
        }
        printf("%d\n", findFinalValue(arr, n, original));
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
        const original = parseInt(input[idx++]);
        const arr = [];
        for (let i = 0; i < n; i++) {
            arr.push(parseInt(input[idx++]));
        }
        console.log(findFinalValue(arr, original));
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
        n, original = map(int, input().split())
        arr = list(map(int, input().split()))
        print(findFinalValue(arr, original))
        # evaluation completed

if __name__ == "__main__":
    main()