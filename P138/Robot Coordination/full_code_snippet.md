## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here


int main() {
    int t;
    cin >> t;

    while (t--) {
        long long x, m;
        cin >> x >> m;
        cout << countCompatible(x, m) << "\n";
    
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
            long x = sc.nextLong();
            long m = sc.nextLong();
            System.out.println(countCompatible(x, m));
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
        long long x, m;
        scanf("%lld %lld", &x, &m);
        printf("%lld\n", countCompatible(x, m));
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
        const x = BigInt(input[idx++]);
        const m = BigInt(input[idx++]);
        console.log(countCompatible(x, m).toString());
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
        x, m = map(int, input().split())
        print(countCompatible(x, m))
        # evaluation completed

if __name__ == "__main__":
    main()
