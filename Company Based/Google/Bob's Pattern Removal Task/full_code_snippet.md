## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here


int main() {
    int t;
    cin >> t;

    while (t--) {
        string s, part;
        cin >> s >> part;
        cout << removeOccurrences(s, part) << endl;
        
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
            String part = sc.next();

            System.out.println(removeOccurrences(s, part));
            // evaluation completed
        }
        sc.close();
    }
}


## C

#include <stdio.h>
#include <stdlib.h>

// user code comes here

int main() {
    int t;
    scanf("%d", &t);

    while (t--) {
        char s[200005];
        char part[200005];

        scanf("%s %s", s, part);

        char* result = removeOccurrences(s, part);
        printf("%s\n", result);
        // evaluation completed

        free(result); // important if malloc is used inside
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
        const s = input[idx++];
        const part = input[idx++];

        console.log(removeOccurrences(s, part));
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
        s, part = input().split()
        print(removeOccurrences(s, part))
        # evaluation completed

if __name__ == "__main__":
    main()
