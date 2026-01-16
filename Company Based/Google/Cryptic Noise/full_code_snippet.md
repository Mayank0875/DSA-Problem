## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here


int main() {
    int t;
    cin >> t;

    while (t--) {
        string s, t;
        cin >> s >> t;
        cout << solve(s, t) << "\n";
    
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
        int tc = sc.nextInt();

        while (tc-- > 0) {
            String s = sc.next();
            String t = sc.next();

            System.out.println(solve(s, t));
            // evaluation completed
        }
        sc.close();
    }
}


## C

#include <stdio.h>

// user code comes here

int main() {
    int tc;
    scanf("%d", &tc);

    while (tc--) {
        char s[200005];
        char t[200005];

        scanf("%s %s", s, t);
        printf("%d\n", solve(s, t));
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

    const tc = Number(input[idx++]);
    for (let i = 0; i < tc; i++) {
        const s = input[idx++];
        const t = input[idx++];

        console.log(solve(s, t));
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
    tc = int(input())
    for _ in range(tc):
        s, t = input().split()
        print(solve(s, t))
        # evaluation completed

if __name__ == "__main__":
    main()
