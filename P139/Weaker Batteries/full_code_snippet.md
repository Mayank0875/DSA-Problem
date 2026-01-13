## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here


int main() {
    int t;
    cin >> t;

    while (t--) {
        int n;
        if (cin >> n) {
            vector<vector<int>> properties(n, vector<int>(2));
            for (int i = 0; i < n; ++i) {
                cin >> properties[i][0] >> properties[i][1];
            }
            cout << numberOfWeakCharacters(properties) << endl;
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
            int[][] properties = new int[n][2];

            for (int i = 0; i < n; i++) {
                properties[i][0] = sc.nextInt();
                properties[i][1] = sc.nextInt();
            }

            System.out.println(numberOfWeakCharacters(properties));
            // evaluation completed
        }
        sc.close();
    }
}


## C

#include <stdio.h>

// user code comes here

int main() {
    int t;
    scanf("%d", &t);

    while (t--) {
        int n;
        scanf("%d", &n);

        int properties[n][2];
        for (int i = 0; i < n; i++) {
            scanf("%d %d", &properties[i][0], &properties[i][1]);
        }

        // convert to int**
        int* ptrs[n];
        for (int i = 0; i < n; i++) {
            ptrs[i] = properties[i];
        }

        printf("%d\n", numberOfWeakCharacters(ptrs, n));
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
        const properties = [];

        for (let i = 0; i < n; i++) {
            const a = Number(input[idx++]);
            const b = Number(input[idx++]);
            properties.push([a, b]);
        }

        console.log(numberOfWeakCharacters(properties));
        // evaluation completed
    }
}

main();


## PYTHON

import math
from typing import List

# user code comes here

def main():
    t = int(input())
    for _ in range(t):
        n = int(input())
        properties = []
        for _ in range(n):
            a, b = map(int, input().split())
            properties.append([a, b])

        print(numberOfWeakCharacters(properties))
        # evaluation completed

if __name__ == "__main__":
    main()
