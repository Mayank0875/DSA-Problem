## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here

int main() {
    int n;
    cin >> n;
    vector<int> arr(n);
    for (int i = 0; i < n; i++) {
        cin >> arr[i];
    }

    int q; cin >> q;
    vector<vector<int>> queries(q, vector<int>(3, 0));

    for(int i = 0; i < q; ++i){
        cin >> queries[i][0] >> queries[i][1] >> queries[i][2];
    }

    long long result = ZeroOneQuery(arr, queries);
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
        int[] arr = new int[n];
        for (int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }

        int q = sc.nextInt();
        int[][] queries = new int[q][3];
        for (int i = 0; i < q; i++) {
            queries[i][0] = sc.nextInt();
            queries[i][1] = sc.nextInt();
            queries[i][2] = sc.nextInt();
        }

        System.out.println(ZeroOneQuery(arr, queries));
        sc.close();
    }
}


## C

#include <stdio.h>
#include <stdlib.h>

// user code comes here

int main() {
    int n;
    scanf("%d", &n);
    int* arr = (int*)malloc(n * sizeof(int));
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    int q;
    scanf("%d", &q);
    int queries[q][3];
    for (int i = 0; i < q; i++) {
        scanf("%d %d %d", &queries[i][0], &queries[i][1], &queries[i][2]);
    }

    long long result = ZeroOneQuery(arr, n, queries, q);
    printf("%lld\n", result);
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
    const arr = input.slice(idx, idx + n);
    idx += n;

    const q = input[idx++];
    const queries = [];
    for (let i = 0; i < q; i++) {
        queries.push([input[idx++], input[idx++], input[idx++]]);
    }

    console.log(ZeroOneQuery(arr, queries));
}

main();



## PYTHON

# user code comes here

def main():
    n = int(input())
    arr = list(map(int, input().split()))

    q = int(input())
    queries = []
    for _ in range(q):
        queries.append(list(map(int, input().split())))

    print(ZeroOneQuery(arr, queries))

if __name__ == "__main__":
    main()