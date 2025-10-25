## CPP

#include <bits/stdc++.h>
using namespace std;

// User function to implement


int main() {
    int t;
    cin >> t;

    while (t--) {
        long long x;
        cin >> x;
        cout << TableMultiplication(x) << "\n";
        
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
            long x = sc.nextLong();
            System.out.println(TableMultiplication(x));
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
        long long x;
        scanf("%lld", &x);
        printf("%lld\n", TableMultiplication(x));
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
        const x = BigInt(input[idx++]);
        console.log(TableMultiplication(x).toString());
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
        x = int(input())
        print(TableMultiplication(x))
        # evaluation completed

if __name__ == "__main__":
    main()