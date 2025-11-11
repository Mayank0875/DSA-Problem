## CPP

#include <bits/stdc++.h>
using namespace std;

// User function to implement


int main() {
    int t;
    cin >> t;

    while (t--) {
        long long w, h, n;
        cin >> w >> h >> n;
        cout << findMinSquareSide(w, h, n) << "\n";
        
        // evaluation completed
    }
    return 0;
}

## JAVA

import java.util.*;

public class Main {
    // User function to implement


    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int t = sc.nextInt();

        while (t-- > 0) {
            long w = sc.nextLong();
            long h = sc.nextLong();
            long n = sc.nextLong();
            System.out.println(findMinSquareSide(w, h, n));
            
            // evaluation completed
        }
        sc.close();
    }
}

## C

#include <stdio.h>
#include <stdbool.h>
#include <stdlib.h>

// User function to implement


int main() {
    int t;
    scanf("%d", &t);

    while (t--) {
        long long w, h, n;
        scanf("%lld %lld %lld", &w, &h, &n);
        printf("%lld\n", findMinSquareSide(w, h, n));
        
        // evaluation completed
    }
    return 0;
}

## JAVASCRIPT

// User function to implement


function main() {
    const fs = require("fs");
    const input = fs.readFileSync(0, "utf-8").trim().split(/\s+/);
    let idx = 0;

    const t = parseInt(input[idx++]);
    for (let tc = 0; tc < t; tc++) {
        const w = BigInt(input[idx++]);
        const h = BigInt(input[idx++]);
        const n = BigInt(input[idx++]);
        console.log(findMinSquareSide(w, h, n).toString());
        
        // evaluation completed
    }
}

main();

## PYTHON
from typing import List
import collections

# User function to implement

def main():
    t = int(input())
    for _ in range(t):
        w, h, n = map(int, input().split())
        print(findMinSquareSide(w, h, n))
        
        # evaluation completed

if __name__ == "__main__":
    main()