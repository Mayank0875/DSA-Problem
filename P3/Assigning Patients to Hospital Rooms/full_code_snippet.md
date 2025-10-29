## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here

int main() {
    int t;
    cin >> t;
    while(t--){
        int n, x;
        cin >> n >> x;
        vector<int> arr(n);
        for (int i = 0; i < n; i++) {
            cin >> arr[i];
        }

        int result = solveFerrisWheel(n, x, arr);
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
            int x = sc.nextInt();
            int[] arr = new int[n];
            for (int i = 0; i < n; i++) arr[i] = sc.nextInt();

            int result = solveFerrisWheel(n, x, arr);
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

int main() {
    int t;
    scanf("%d", &t);

    while (t--) {
        int n, x;
        scanf("%d %d", &n, &x);
        int* arr = (int*)malloc(n * sizeof(int));
        for (int i = 0; i < n; i++) scanf("%d", &arr[i]);

        int result = solveFerrisWheel(n, x, arr);
        printf("%d\n", result);

        free(arr);

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
        const x = input[idx++];
        const arr = input.slice(idx, idx + n);
        idx += n;

        const result = solveFerrisWheel(n, x, arr);
        console.log(result);

        // evaluation completed
    }
}

main();

## PYTHON

from typing import List

# user code comes here

def main():
    t = int(input())
    for _ in range(t):
        n, x = map(int, input().split())
        arr = list(map(int, input().split()))

        result = solveFerrisWheel(n, x, arr)
        print(result)

        # evaluation completed

if __name__ == "__main__":
    main()