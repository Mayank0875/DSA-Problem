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
        vector<int> arr(n);
        for (int i = 0; i < n; ++i) cin >> arr[i];

        vector<int> result = sortByBits(arr);
        for (int x : result) cout << x << " ";
        cout << "\n";
        
        // evaluation completed
    }
    return 0;
}


## JAVA

import java.util.*;

public class Main {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int t = sc.nextInt();

        while (t-- > 0) {
            int n = sc.nextInt();
            int[] arr = new int[n];
            for (int i = 0; i < n; i++) arr[i] = sc.nextInt();

            int[] result = sortByBits(arr);
            for (int x : result) System.out.print(x + " ");
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
        for (int i = 0; i < n; i++) scanf("%d", &arr[i]);

        sortByBits(arr, n);
        for (int i = 0; i < n; i++) printf("%d ", arr[i]);
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
        const arr = [];
        for (let i = 0; i < n; i++) arr.push(parseInt(input[idx++]));

        const result = sortByBits(arr);
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
        result = sortByBits(arr)
        print(*result)
        # evaluation completed

if __name__ == "__main__":
    main()
