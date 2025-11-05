## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here


int main() {
    int t = 1;
    cin >> t;

    while (t--) {
        int n; cin >> n;
        int res = countWellFormed(n);
        cout << res << endl;
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
        int t = 1;
        if (sc.hasNextInt()) t = sc.nextInt();

        while (t-- > 0) {
            int n = sc.nextInt();
            int res = countWellFormed(n);
            System.out.println(res);
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
    int t = 1;
    scanf("%d", &t);

    while (t--) {
        int n;
        scanf("%d", &n);
        int res = countWellFormed(n);
        printf("%d\n", res);
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

    let t = 1;
    if (idx < input.length) t = parseInt(input[idx++]);

    for (let tc = 0; tc < t; tc++) {
        const n = parseInt(input[idx++]);
        const res = countWellFormed(n);
        console.log(res);
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
        res = countWellFormed(n)
        print(res)
        # evaluation completed

if __name__ == "__main__":
    main()
