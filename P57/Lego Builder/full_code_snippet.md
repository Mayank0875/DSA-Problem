## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here

int main() {
    int t;
    cin >> t;

    while (t--) {
        int n; 
        cin >> n;
        vector<string> arr(n);
        for (int i = 0; i < n; ++i) {
            cin >> arr[i];
        }
        string s; 
        cin >> s;
        cout << countValidSpells(arr, s) << "\n";
        
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
            int n = sc.nextInt();
            String[] arr = new String[n];
            for (int i = 0; i < n; i++) {
                arr[i] = sc.next();
            }
            String s = sc.next();
            System.out.println(countValidSpells(arr, s));
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
        int n;
        scanf("%d", &n);
        char** arr = (char**)malloc(n * sizeof(char*));
        for (int i = 0; i < n; i++) {
            arr[i] = (char*)malloc(1001 * sizeof(char));
            scanf("%s", arr[i]);
        }
        char s[1001];
        scanf("%s", s);
        printf("%d\n", countValidSpells(n, arr, s));
        
        // Free allocated memory
        for (int i = 0; i < n; i++) {
            free(arr[i]);
        }
        free(arr);

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
        const n = parseInt(input[idx++]);
        const arr = [];
        for (let i = 0; i < n; i++) {
            arr.push(input[idx++]);
        }
        const s = input[idx++];
        console.log(countValidSpells(arr, s));
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
        arr = [input().strip() for _ in range(n)]
        s = input().strip()
        print(countValidSpells(arr, s))
        # evaluation completed

if __name__ == "__main__":
    main()