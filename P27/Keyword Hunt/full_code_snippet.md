## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here


int main() {
    int t;
    cin >> t;

    while (t--) {
        int n, m; cin >> n >> m;
        vector<vector<char>> grid(n, vector<char> (m));

        for(int i = 0; i < n; ++i){
            for(int j = 0; j < m; ++j){
                cin >> grid[i][j];
            }
        }
        string word; cin >> word;
        
        if(exist(grid, word)) {
            cout << "Yes" << endl;
        } else {
            cout << "No" << endl;
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
            int n = sc.nextInt();
            int m = sc.nextInt();
            char[][] grid = new char[n][m];

            for (int i = 0; i < n; i++) {
                for (int j = 0; j < m; j++) {
                    grid[i][j] = sc.next().charAt(0);
                }
            }

            String word = sc.next();

            if (exist(grid, word)) {
                System.out.println("Yes");
            } else {
                System.out.println("No");
            }

            // evaluation completed
        }
        sc.close();
    }
}


## C

#include <stdio.h>
#include <stdbool.h>
#include <stdlib.h>
#include <string.h>

// user code comes here

int main() {
    int t;
    scanf("%d", &t);

    while (t--) {
        int n, m;
        scanf("%d %d", &n, &m);

        char** board = (char**)malloc(n * sizeof(char*));
        for (int i = 0; i < n; i++) {
            board[i] = (char*)malloc((m + 1) * sizeof(char));
            for (int j = 0; j < m; j++) {
                scanf(" %c", &board[i][j]);
            }
        }

        char word[1005];
        scanf("%s", word);
        int* boardColSize = (int*)malloc(n * sizeof(int));
        for (int i = 0; i < n; i++) boardColSize[i] = m;

        if (exist(board, n, boardColSize, word)) {
            printf("Yes\n");
        } else {
            printf("No\n");
        }

        for (int i = 0; i < n; i++) free(board[i]);
        free(board);
        free(boardColSize);

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
        const m = parseInt(input[idx++]);
        const grid = Array.from({ length: n }, () => Array(m));

        for (let i = 0; i < n; i++) {
            for (let j = 0; j < m; j++) {
                grid[i][j] = input[idx++];
            }
        }

        let word = input[idx++];

        if (exist(grid, word)) {
            console.log("Yes");
        } else {
            console.log("No");
        }

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
        n, m = map(int, input().split())
        grid = [list(input().split()) for _ in range(n)]
        word = input().strip()

        if exist(grid, word):
            print("Yes")
        else:
            print("No")

        # evaluation completed

if __name__ == "__main__":
    main()
