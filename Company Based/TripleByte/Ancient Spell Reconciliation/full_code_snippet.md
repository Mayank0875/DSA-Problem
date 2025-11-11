## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here


int main() {
    int t;
    cin >> t;

    while (t--) {
        string s1, s2;
        cin >> s1 >> s2;
        cout << minDeleteSum(s1, s2) << "\n";
        
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
            String s1 = sc.next();
            String s2 = sc.next();
            System.out.println(minDeleteSum(s1, s2));
            // evaluation completed
        }
        sc.close();
    }
}

## C

#include <stdio.h>
#include <stdlib.h>
#include <string.h>

// user code comes here

int main() {
    int t;
    scanf("%d", &t);
    while (t--) {
        char s1[1001], s2[1001];
        scanf("%s %s", s1, s2);
        printf("%d\n", minDeleteSum(s1, s2));
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
        const s1 = input[idx++];
        const s2 = input[idx++];
        console.log(minDeleteSum(s1, s2));
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
        s1 = input().strip()
        s2 = input().strip()
        print(minDeleteSum(s1, s2))
        # evaluation completed

if __name__ == "__main__":
    main()