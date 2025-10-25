## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here


int main() {
    int t;
    cin >> t;

    while (t--) {
        long long x;
        cin >> x;
        cout << integerSquareRoot(x) << "\n";
        
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
            System.out.println(integerSquareRoot(x));
            // evaluation completed
        }
        sc.close();
    }
}

## C

#include <stdio.h>
#include <stdbool.h>
#include <stdlib.h>

// user code comes here


int main() {
    int t;
    scanf("%d", &t);
    while (t--) {
        long long x;
        scanf("%lld", &x);
        printf("%lld\n", integerSquareRoot(x));
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
        const x = BigInt(input[idx++]);
        console.log(integerSquareRoot(x).toString());
        // evaluation completed
    }
}

main();

## PYTHON
import collections

# user code comes here


def main():
    t = int(input())
    for _ in range(t):
        x = int(input())
        print(integerSquareRoot(x))
        # evaluation completed

if __name__ == "__main__":
    main()