## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here

int main() {
    int n, k;
    cin >> n >> k;
    vector<int> arr(n);
    for (int i = 0; i < n; i++) {
        cin >> arr[i];
    }

    int result = XorofXoR(arr, k);
    cout << result << endl;

    return 0;
}

## JAVA

import java.util.*;

public class Main {
    // user code comes here

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int k = sc.nextInt();
        int[] arr = new int[n];
        for (int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }

        int result = XorofXoR(arr, k);
        System.out.println(result);

        sc.close();
    }
}

## C

#include <stdio.h>
#include <stdlib.h>

// user code comes here

int main() {
    int n, k;
    scanf("%d %d", &n, &k);
    int* arr = (int*)malloc(n * sizeof(int));
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    int result = XorofXoR(arr, n, k);
    printf("%d\n", result);

    free(arr);
    return 0;
}

## JAVASCRIPT

// user code comes here

function main() {
    const fs = require("fs");
    const input = fs.readFileSync(0, "utf-8").trim().split(/\s+/).map(Number);

    let idx = 0;
    const n = input[idx++];
    const k = input[idx++];
    const arr = input.slice(idx, idx + n);

    const result = XorofXoR(arr, k);
    console.log(result);
}

main();



## PYTHON

from typing import List

# user code comes here

def main():
    n, k = map(int, input().split())
    arr = list(map(int, input().split()))

    result = XorofXoR(arr, k)
    print(result)

if __name__ == "__main__":
    main()