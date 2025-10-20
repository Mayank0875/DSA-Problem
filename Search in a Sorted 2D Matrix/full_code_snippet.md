## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here

int main() {
    int t;
    cin >> t;
    while(t--){
        int n, m, target;
        cin >> m >> n >> target;
        vector<vector<int>> grid(m, vector<int>(n, 0));
        
        for(int i = 0; i < m; ++i){
            for(int j = 0; j < n; ++j){
                cin >> grid[i][j];
            }
        }

        int result = searchMatrix(arr, target);
        cout << result << endl;

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
        while(t-- > 0){
            int m = sc.nextInt();
            int n = sc.nextInt();
            int target = sc.nextInt();
            int[][] grid = new int[m][n];

            for(int i = 0; i < m; i++){
                for(int j = 0; j < n; j++){
                    grid[i][j] = sc.nextInt();
                }
            }

            int result = searchMatrix(grid, target);
            System.out.println(result);

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
    while(t--){
        int m, n, target;
        scanf("%d %d %d", &m, &n, &target);
        int grid[m][n];
        for(int i = 0; i < m; i++){
            for(int j = 0; j < n; j++){
                scanf("%d", &grid[i][j]);
            }
        }

        int result = searchMatrix(m, n, grid, target);
        printf("%d\n", result);

        // evaluation completed
    }
    return 0;
}


## JAVASCRIPT

// user code comes here

function main() {
    const fs = require("fs");
    const input = fs.readFileSync(0, "utf-8").trim().split(/\s+/).map(Number);

    let idx = 0;
    const t = input[idx++];

    for (let test = 0; test < t; test++) {
        const m = input[idx++];
        const n = input[idx++];
        const target = input[idx++];
        const grid = [];

        for (let i = 0; i < m; i++) {
            const row = input.slice(idx, idx + n);
            idx += n;
            grid.push(row);
        }

        const result = searchMatrix(grid, target);
        console.log(result);

        // evaluation completed
    }
}

main();


## PYTHON

from typing import List

# user code comes here

def main():
    t = int(input())
    for _ in range(t):
        m, n, target = map(int, input().split())
        grid = [list(map(int, input().split())) for _ in range(m)]
        result = searchMatrix(grid, target)
        print(result)

        # evaluation completed

if __name__ == "__main__":
    main()

