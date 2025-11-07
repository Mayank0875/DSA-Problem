## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here


int main() {
    int t;
    cin >> t;

    while (t--) {
        string s;
        cin >> s;
        cout << scoreOfParentheses(s) << "\n";
        
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
            String s = sc.next();
            System.out.println(scoreOfParentheses(s));
            // evaluation completed
        }
        sc.close();
    }
}


## C

#include <stdio.h>
#include <stdlib.h>
#include <string.h>
#include <math.h>

// user code comes here


int main() {
    int t;
    scanf("%d", &t);
    while (t--) {
        char s[1005];
        scanf("%s", s);
        printf("%d\n", scoreOfParentheses(s));
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
        const s = input[idx++];
        console.log(scoreOfParentheses(s));
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
        s = input().strip()
        print(scoreOfParentheses(s))
        # evaluation completed

if __name__ == "__main__":
    main()
