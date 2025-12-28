## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here


int main() {
    int t;
    cin >> t;

    while (t--) {
        int n;
        if (!(cin >> n)) return 0;
        
        vector<int> prices(n);
        for (int i = 0; i < n; i++) {
            cin >> prices[i];
        }
        
        cout << maxProfit(prices) << endl;
        
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
            int[] prices = new int[n];

            for (int i = 0; i < n; i++) {
                prices[i] = sc.nextInt();
            }

            System.out.println(maxProfit(prices));

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
        if (scanf("%d", &n) != 1) return 0;

        int* prices = (int*)malloc(n * sizeof(int));
        for (int i = 0; i < n; i++) {
            scanf("%d", &prices[i]);
        }

        printf("%d\n", maxProfit(prices, n));

        free(prices);

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

    const t = Number(input[idx++]);

    for (let tc = 0; tc < t; tc++) {
        const n = Number(input[idx++]);
        const prices = new Array(n);

        for (let i = 0; i < n; i++) {
            prices[i] = Number(input[idx++]);
        }

        console.log(maxProfit(prices));

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
        prices = list(map(int, input().split()))

        print(maxProfit(prices))

        # evaluation completed

if __name__ == "__main__":
    main()
