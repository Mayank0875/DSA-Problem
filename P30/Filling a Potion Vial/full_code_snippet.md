## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here


int main() {
    int t = 1;
    cin >> t;

    while (t--) {
        int n, tar; cin >> n >> tar;
        vector<int> arr(n);
        for (int i = 0; i < n; ++i) {
            cin >> arr[i];
        }
        int res = countCombinations(arr, tar);
        cout << res << endl;
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
        int t = 1;
        if (sc.hasNextInt()) t = sc.nextInt();

        while (t-- > 0) {
            int n = sc.nextInt();
            int tar = sc.nextInt();
            int[] arr = new int[n];
            for (int i = 0; i < n; i++) arr[i] = sc.nextInt();
            int res = countCombinations(arr, tar);
            System.out.println(res);
            // evaluation completed
        }
        sc.close();
    }
}



## C

#include <stdio.h>
#include <stdbool.h>

// user code comes here

int main() {
    int t = 1;
    scanf("%d", &t);

    while (t--) {
        int n, tar;
        scanf("%d %d", &n, &tar);
        int arr[n];
        for (int i = 0; i < n; i++) scanf("%d", &arr[i]);
        int res = countCombinations(arr, n, tar);
        printf("%d\n", res);
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

    let t = 1;
    if (idx < input.length) t = parseInt(input[idx++]);

    for (let tc = 0; tc < t; tc++) {
        const n = parseInt(input[idx++]);
        const tar = parseInt(input[idx++]);
        const arr = [];
        for (let i = 0; i < n; i++) arr.push(parseInt(input[idx++]));
        const res = countCombinations(arr, tar);
        console.log(res);
        // evaluation completed
    }
}

main();



## PYTHON

# user code comes here

def main():
    t = int(input())
    for _ in range(t):
        n, tar = map(int, input().split())
        arr = list(map(int, input().split()))
        res = countCombinations(arr, tar)
        print(res)
        # evaluation completed

if __name__ == "__main__":
    main()

