## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here



int main() {
    int t = 1;
    cin >> t;

    while (t--) {
        int n;
        long long sum; 
        cin >> n >> sum;
        vector<long long> arr(n);

        for(int i = 0; i < n; ++i){
            cin >> arr[i];
        }
        
        if(hasSubsetSum(arr, sum)) {
            cout << "Yes" << endl;
        } else {
            cout << "No" << endl;
        }
        
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
            long sum = sc.nextLong();
            long[] arr = new long[n];
            for (int i = 0; i < n; ++i) {
                arr[i] = sc.nextLong();
            }

            if (hasSubsetSum(arr, sum))
                System.out.println("Yes");
            else
                System.out.println("No");

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
    int t;
    scanf("%d", &t);

    while (t--) {
        int n;
        long long sum;
        scanf("%d %lld", &n, &sum);
        long long arr[n];
        for (int i = 0; i < n; ++i) {
            scanf("%lld", &arr[i]);
        }

        if (hasSubsetSum(arr, n, sum))
            printf("Yes\n");
        else
            printf("No\n");

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
        const sum = Number(input[idx++]);
        const arr = [];
        for (let i = 0; i < n; i++) {
            arr.push(Number(input[idx++]));
        }

        if (hasSubsetSum(arr, sum)) console.log("Yes");
        else console.log("No");

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
        n, total_sum = map(int, input().split())
        arr = list(map(int, input().split()))

        if hasSubsetSum(arr, total_sum):
            print("Yes")
        else:
            print("No")

        # evaluation completed


if __name__ == "__main__":
    main()