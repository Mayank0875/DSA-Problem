## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here

int main() {
    int t;
    cin >> t;
    while (t--) {
        int n;
        long long target;
        cin >> n >> target;
        vector<int> arr(n);
        for (int i = 0; i < n; i++) {
            cin >> arr[i];
        }

        long long result = MinimumTime(n, target, arr);
        cout << result << endl;

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

            long result = MinimumTime(n, target, arr);
            System.out.println(result);

            // evaluation completed
        }
        sc.close();
    }
}

## C

#include <stdio.h>
#include <stdlib.h>

// user code comes here

long long MinimumTime(int n, long long target, int arr[]);

int main() {
    int t;
    scanf("%d", &t);
    while (t--) {
        int n;
        long long target;
        scanf("%d %lld", &n, &target);
        int arr[n];
        for (int i = 0; i < n; i++) {
            scanf("%d", &arr[i]);
        }

        long long result = MinimumTime(n, target, arr);
        printf("%lld\n", result);

        // evaluation completed
    }
    return 0;
}


## JAVASCRIPT

// user code comes here

function main() {
    const fs = require("fs");
    const input = fs.readFileSync(0, "utf-8").trim().split(/\s+/).map(Number);

    let idx = 0;
    const t = input[idx++];

    for (let test = 0; test < t; test++) {
        const n = input[idx++];
        const target = BigInt(input[idx++]);
        const arr = input.slice(idx, idx + n).map(Number);
        idx += n;

        const result = MinimumTime(n, target, arr);
        console.log(result.toString());

        // evaluation completed
    }
}

main();

## PYTHON

from typing import List
import collections

# user code comes here

def main():
    t = int(input())
    for _ in range(t):
        n, target = map(int, input().split())
        arr = list(map(int, input().split()))

        result = MinimumTime(n, target, arr)
        print(result)

        # evaluation completed

if __name__ == "__main__":
    main()