## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here


int main() {
    int t;
    cin >> t;

    while (t--) {
        int n; long long target; 
        cin >> n;
        cin >> target;
        vector<int> arr(n);
        for (int i = 0; i < n; ++i) cin >> arr[i];
        cout << countConstellations(arr, target) << "\n";
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
            long target = sc.nextLong();
            int[] arr = new int[n];
            
            for (int i = 0; i < n; i++) {
                arr[i] = sc.nextInt();
            }

            System.out.println(countConstellations(arr, target));
            // evaluation completed
        }
        
        sc.close();
    }
}


## C

#include <stdio.h>
#include <stdlib.h>
#include <math.h>
#include <stdbool.h>

// user code comes here


int main() {
    int t;
    scanf("%d", &t);

    while (t--) {
        int n;
        long long target;
        scanf("%d %lld", &n, &target);

        int* arr = (int*)malloc(n * sizeof(int));
        for (int i = 0; i < n; i++) {
            scanf("%d", &arr[i]);
        }

        printf("%lld\n", countConstellations(arr, n, target));
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
        const target = BigInt(input[idx++]);
        const arr = [];
        for (let i = 0; i < n; i++) {
            arr.push(parseInt(input[idx++]));
        }

        console.log(countConstellations(arr, target).toString());
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
        n, target = map(int, input().split())
        arr = list(map(int, input().split()))
        print(countConstellations(arr, target))
        # evaluation completed


if __name__ == "__main__":
    main()
