## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here


int main() {
    int t;
    cin >> t;

    while (t--) {
        int a, b;
        cin >> a >> b;
        cout << maxRounds(a, b) << "\n";
        
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
            int a = sc.nextInt();
            int b = sc.nextInt();

            System.out.println(maxRounds(a, b));
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
        int a, b;
        scanf("%d %d", &a, &b);

        printf("%d\n", maxRounds(a, b));
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
        const a = Number(input[idx++]);
        const b = Number(input[idx++]);

        console.log(maxRounds(a, b));
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
        a, b = map(int, input().split())
        print(maxRounds(a, b))
        # evaluation completed

if __name__ == "__main__":
    main()
