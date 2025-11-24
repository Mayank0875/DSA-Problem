## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here

int main() {
    int t; 
    cin >> t;

    while(t--){
        int n;
        cin >> n;
        vector<int> arr(n);
        for (int i = 0; i < n; i++) {
            cin >> arr[i];
        }

        int q; cin >> q;
        vector<vector<int>> queries(q, vector<int>(2, 0));

        for(int i = 0; i < q; ++i){
            cin >> queries[i][0] >> queries[i][1];
        }

        vector<int> result = sumEvenAfterQueries(arr, queries);
        for(auto val : result){
            cout << val << ' ';
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

        while(t-- > 0){
            int n = sc.nextInt();
            int[] arr = new int[n];
            for (int i = 0; i < n; i++) {
                arr[i] = sc.nextInt();
            }

            int q = sc.nextInt();
            int[][] queries = new int[q][2];
            for (int i = 0; i < q; i++) {
                queries[i][0] = sc.nextInt();
                queries[i][1] = sc.nextInt();
            }

            int[] result = sumEvenAfterQueries(arr, queries);
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

    while(t--){
        int n;
        scanf("%d", &n);
        int* arr = (int*)malloc(n * sizeof(int));
        for (int i = 0; i < n; i++) {
            scanf("%d", &arr[i]);
        }

        int q;
        scanf("%d", &q);
        int** queries = (int**)malloc(q * sizeof(int*));
        for (int i = 0; i < q; i++) {
            queries[i] = (int*)malloc(2 * sizeof(int));
            scanf("%d %d", &queries[i][0], &queries[i][1]);
        }

        int returnSize;
        int* result = sumEvenAfterQueries(arr, n, queries, q, &returnSize);
        for (int i = 0; i < returnSize; i++) {
            printf("%d ", result[i]);
        }
        printf("\n");

        free(arr);
        for (int i = 0; i < q; i++) {
            free(queries[i]);
        }
        free(queries);
        free(result);

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

    for(let test = 0; test < t; test++){
        const n = input[idx++];
        const arr = input.slice(idx, idx + n);
        idx += n;

        const q = input[idx++];
        const queries = [];
        for (let i = 0; i < q; i++) {
            queries.push([input[idx++], input[idx++]]);
        }

        const result = sumEvenAfterQueries(arr, queries);
        console.log(result.join(" "));

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
        n = int(input())
        arr = list(map(int, input().split()))

        q = int(input())
        queries = []
        for _ in range(q):
            queries.append(list(map(int, input().split())))

        result = sumEvenAfterQueries(arr, queries)
        print(" ".join(map(str, result)))

        # evaluation completed

if __name__ == "__main__":
    main()