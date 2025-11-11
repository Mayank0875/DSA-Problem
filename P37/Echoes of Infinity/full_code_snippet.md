## CPP

#include <bits/stdc++.h>
using namespace std;

// User function to implement


int main() {
    int t;
    cin >> t;

    while (t--) {
        long long n, x, y;
        cin >> n >> x >> y;
        cout << MinimumTime(n, x, y) << "\n";
        
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
            long n = sc.nextLong();
            long x = sc.nextLong();
            long y = sc.nextLong();
            System.out.println(MinimumTime(n, x, y));
            
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
        long long n, x, y;
        scanf("%lld %lld %lld", &n, &x, &y);
        printf("%lld\n", MinimumTime(n, x, y));
        
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
        const n = BigInt(input[idx++]);
        const x = BigInt(input[idx++]);
        const y = BigInt(input[idx++]);
        console.log(MinimumTime(n, x, y).toString());
        
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
        n, x, y = map(int, input().split())
        print(MinimumTime(n, x, y))
        
        # evaluation completed

if __name__ == "__main__":
    main()