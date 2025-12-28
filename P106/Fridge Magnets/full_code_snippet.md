## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here


int main() {
    int t;
    cin >> t;

    while (t--) {
        int m, n;
        if (!(cin >> m >> n)) return 0;
        
        vector<vector<char>> box(m, vector<char>(n));
        for (int i = 0; i < m; i++) {
            for (int j = 0; j < n; j++) {
                cin >> box[i][j];
            }
        }

        vector<vector<char>> result = rotateTheBox(box);
        
        for (const auto& row : result) {
            for (size_t j = 0; j < row.size(); j++) {
                cout << row[j] << (j == row.size() - 1 ? "" : " ");
            }
            cout << endl;
        }
        
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
            int m = sc.nextInt();
            int n = sc.nextInt();

            char[][] box = new char[m][n];
            for (int i = 0; i < m; i++) {
                for (int j = 0; j < n; j++) {
                    box[i][j] = sc.next().charAt(0);
                }
            }

            char[][] result = rotateTheBox(box);

            for (int i = 0; i < result.length; i++) {
                for (int j = 0; j < result[i].length; j++) {
                    System.out.print(result[i][j]);
                    if (j + 1 < result[i].length) System.out.print(" ");
                }
                System.out.println();
            }

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
        int m, n;
        if (scanf("%d %d", &m, &n) != 2) return 0;

        char** box = (char**)malloc(m * sizeof(char*));
        for (int i = 0; i < m; i++) {
            box[i] = (char*)malloc(n * sizeof(char));
            for (int j = 0; j < n; j++) {
                scanf(" %c", &box[i][j]);
            }
        }

        char** result = rotateTheBox(box, m, n);

        for (int i = 0; i < n; i++) {
            for (int j = 0; j < m; j++) {
                printf("%c", result[i][j]);
                if (j + 1 < m) printf(" ");
            }
            printf("\n");
        }

        for (int i = 0; i < m; i++) free(box[i]);
        free(box);

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
        const m = Number(input[idx++]);
        const n = Number(input[idx++]);

        const box = Array.from({ length: m }, () => Array(n));
        for (let i = 0; i < m; i++) {
            for (let j = 0; j < n; j++) {
                box[i][j] = input[idx++];
            }
        }

        const result = rotateTheBox(box);

        for (const row of result) {
            console.log(row.join(" "));
        }

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
        m, n = map(int, input().split())
        box = []

        for _ in range(m):
            box.append(input().split())

        result = rotateTheBox(box)

        for row in result:
            print(" ".join(row))

        # evaluation completed

if __name__ == "__main__":
    main()
