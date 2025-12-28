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

        vector<int> apprentices(n);
        for (int i = 0; i < n; i++) {
            cin >> apprentices[i];
        }

        vector<int> potions(n);
        for (int i = 0; i < n; i++) {
            cin >> potions[i];
        }

        int result = countUnluckyApprentices(apprentices, potions);
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
        Scanner scanner = new Scanner(System.in);
        int t = scanner.nextInt();
        while (t-- > 0) {
            int n = scanner.nextInt();
            int[] apprentices = new int[n];
            for (int i = 0; i < n; i++) {
                apprentices[i] = scanner.nextInt();
            }

            int[] potions = new int[n];
            for (int i = 0; i < n; i++) {
                potions[i] = scanner.nextInt();
            }

            int result = countUnluckyApprentices(apprentices, potions);
            System.out.println(result);
            // evaluation completed
        }
        sc.close();
    }
}

## C

#include <stdio.h>
#include <stdbool.h>
#include <stdlib.h>
#include <math.h>


// user code comes here


int main() {
    int t;
    scanf("%d", &t);
    while (t--) {
        int n;
        if (scanf("%d", &n) != 1) return 0;

        int* apprentices = (int*)malloc(n * sizeof(int));
        for (int i = 0; i < n; i++) {
            scanf("%d", &apprentices[i]);
        }

        int* potions = (int*)malloc(n * sizeof(int));
        for (int i = 0; i < n; i++) {
            scanf("%d", &potions[i]);
        }

        int result = countUnluckyApprentices(apprentices, n, potions, n);
        printf("%d\n", result);

        free(apprentices);
        free(potions);
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

        const apprentices = new Array(n);
        for (let i = 0; i < n; i++) {
            apprentices[i] = Number(input[idx++]);
        }

        const potions = new Array(n);
        for (let i = 0; i < n; i++) {
            potions[i] = Number(input[idx++]);
        }

        const result = countUnluckyApprentices(apprentices, potions);
        console.log(result);

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
        apprentices = list(map(int, input().split()))
        potions = list(map(int, input().split()))

        result = countUnluckyApprentices(apprentices, potions)
        print(result)

        # evaluation completed

if __name__ == "__main__":
    main()
