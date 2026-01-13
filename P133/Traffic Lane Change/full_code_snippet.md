## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here


int main() {
    int t;
    cin >> t;

    while (t--) {
        int n;
        if (cin >> n) {
            string dummy; 
            getline(cin, dummy); // Consume newline after n
            
            vector<vector<int>> wall;
            for(int i = 0; i < n; ++i) {
                string line;
                getline(cin, line);
                stringstream ss(line);
                int val;
                vector<int> row;
                while(ss >> val) {
                    row.push_back(val);
                }
                wall.push_back(row);
            }
            cout << leastBricks(wall) << endl;
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
        int t = Integer.parseInt(sc.nextLine());

        while (t-- > 0) {
            int n = Integer.parseInt(sc.nextLine());

            List<List<Integer>> wall = new ArrayList<>();
            for (int i = 0; i < n; i++) {
                String line = sc.nextLine();
                String[] parts = line.trim().split("\\s+");
                List<Integer> row = new ArrayList<>();
                for (String p : parts) {
                    row.add(Integer.parseInt(p));
                }
                wall.add(row);
            }

            System.out.println(leastBricks(wall));
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
    getchar(); // consume newline

    while (t--) {
        int n;
        scanf("%d", &n);
        getchar(); // consume newline

        int** wall = (int**)malloc(n * sizeof(int*));
        int* wallColSize = (int*)malloc(n * sizeof(int));

        for (int i = 0; i < n; i++) {
            char line[10005];
            fgets(line, sizeof(line), stdin);

            int cap = 10, sz = 0;
            wall[i] = (int*)malloc(cap * sizeof(int));

            char* tok = strtok(line, " ");
            while (tok) {
                if (sz == cap) {
                    cap *= 2;
                    wall[i] = (int*)realloc(wall[i], cap * sizeof(int));
                }
                wall[i][sz++] = atoi(tok);
                tok = strtok(NULL, " ");
            }
            wallColSize[i] = sz;
        }

        printf("%d\n", leastBricks(wall, n, wallColSize));
        // evaluation completed

        for (int i = 0; i < n; i++) free(wall[i]);
        free(wall);
        free(wallColSize);
    }
    return 0;
}


## JAVASCRIPT

// user code comes here

function main() {
    const fs = require("fs");
    const input = fs.readFileSync(0, "utf-8").trimEnd().split("\n");
    let idx = 0;

    const t = Number(input[idx++]);

    for (let tc = 0; tc < t; tc++) {
        const n = Number(input[idx++]);
        const wall = [];

        for (let i = 0; i < n; i++) {
            const row = input[idx++].trim().split(/\s+/).map(Number);
            wall.push(row);
        }

        console.log(leastBricks(wall));
        // evaluation completed
    }
}

main();


## PYTHON

import math
from typing import List
from collections import defaultdict

# user code comes here

def main():
    t = int(input())
    for _ in range(t):
        n = int(input())
        wall = []
        for _ in range(n):
            wall.append(list(map(int, input().split())))

        print(leastBricks(wall))
        # evaluation completed

if __name__ == "__main__":
    main()
