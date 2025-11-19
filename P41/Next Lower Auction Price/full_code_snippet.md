## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here

int main() {
    int t;
    cin >> t;

    while (t--) {
        int n; cin >> n;
        vector<int> arr(n);
        for(int i = 0; i < n; ++i){
            cin >> arr[i];
        }

        vector<int> result = findNextLowerTemperature(arr);

        for(int i = 0; i < n; ++i){
            cout << result[i] << ' ';
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
            List<Integer> arr = new ArrayList<>();
            for (int i = 0; i < n; ++i) {
                arr.add(sc.nextInt());
            }

            List<Integer> result = findNextLowerTemperature(arr);

            for (int val : result) {
                System.out.print(val + " ");
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

        int* arr = (int*)malloc(n * sizeof(int));
        for (int i = 0; i < n; ++i) {
            scanf("%d", &arr[i]);
        }

        int* result = findNextLowerTemperature(arr, n);
        if (result != NULL) {
            for (int i = 0; i < n; ++i) {
                printf("%d ", result[i]);
            }
            printf("\n");
            free(result);
        }

        free(arr);
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
        for (let i = 0; i < n; ++i) {
            arr.push(parseInt(input[idx++]));
        }

        const result = findNextLowerTemperature(arr);
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
        result = findNextLowerTemperature(arr)
        print(*result)
        # evaluation completed

if __name__ == "__main__":
    main()