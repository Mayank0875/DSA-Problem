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

        vector<vector<char>> grid(m, vector<char>(n));
        for (int i = 0; i < m; i++) {
            for (int j = 0; j < n; j++) {
                cin >> grid[i][j];
            }
        }

        cout << numIslands(grid) << endl;
        
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

            char[][] grid = new char[m][n];
            for (int i = 0; i < m; i++) {
                for (int j = 0; j < n; j++) {
                    grid[i][j] = sc.next().charAt(0);
                }
            }

            System.out.println(numIslands(grid));

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

        char** grid = (char**)malloc(m * sizeof(char*));
        for (int i = 0; i < m; i++) {
            grid[i] = (char*)malloc(n * sizeof(char));
            for (int j = 0; j < n; j++) {
                scanf(" %c", &grid[i][j]);
            }
        }

        printf("%d\n", numIslands(grid, m, n));

        for (int i = 0; i < m; i++) {
            free(grid[i]);
        }
        free(grid);

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

        const grid = Array.from({ length: m }, () => Array(n));
        for (let i = 0; i < m; i++) {
            for (let j = 0; j < n; j++) {
                grid[i][j] = input[idx++];
            }
        }

        console.log(numIslands(grid));

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
        grid = []

        for _ in range(m):
            grid.append(input().split())

        print(numIslands(grid))

        # evaluation completed

if __name__ == "__main__":
    main()
