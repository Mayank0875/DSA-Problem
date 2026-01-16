## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here


int main() {
    int t;
    cin >> t;

    while (t--) {
        int mass;
        if (!(cin >> mass)) return 0;
        
        int n;
        cin >> n;
        
        vector<int> asteroids(n);
        for (int i = 0; i < n; i++) {
            cin >> asteroids[i];
        }
        
        bool result = asteroidsDestroyed(mass, asteroids);
        if (result) cout << "true" << endl;
        else cout << "false" << endl;
        
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
            int mass = sc.nextInt();
            int n = sc.nextInt();

            int[] asteroids = new int[n];
            for (int i = 0; i < n; i++) {
                asteroids[i] = sc.nextInt();
            }

            boolean result = asteroidsDestroyed(mass, asteroids);
            System.out.println(result ? "true" : "false");
            // evaluation completed
        }
        sc.close();
    }
}


## C

#include <stdio.h>
#include <stdbool.h>

// user code comes here

int main() {
    int t;
    scanf("%d", &t);

    while (t--) {
        int mass;
        scanf("%d", &mass);

        int n;
        scanf("%d", &n);

        int asteroids[n];
        for (int i = 0; i < n; i++) {
            scanf("%d", &asteroids[i]);
        }

        bool result = asteroidsDestroyed(mass, asteroids, n);
        if (result) printf("true\n");
        else printf("false\n");
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
        const mass = Number(input[idx++]);
        const n = Number(input[idx++]);

        const asteroids = [];
        for (let i = 0; i < n; i++) {
            asteroids.push(Number(input[idx++]));
        }

        const result = asteroidsDestroyed(mass, asteroids);
        console.log(result ? "true" : "false");
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
        mass = int(input())
        n = int(input())
        asteroids = list(map(int, input().split()))

        result = asteroidsDestroyed(mass, asteroids)
        print("true" if result else "false")
        # evaluation completed

if __name__ == "__main__":
    main()
