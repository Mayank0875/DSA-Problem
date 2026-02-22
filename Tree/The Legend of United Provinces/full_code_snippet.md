## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here


int main() {
    int t;
    cin >> t;

    while (t--) {
        int n;
        std::cin >> n;
        std::vector<std::vector<int>> matrix(n, std::vector<int>(n));
        for(int i = 0; i < n; i++) {
            for(int j = 0; j < n; j++) {
                std::cin >> matrix[i][j];
            }
        }
        std::cout << solve(matrix) << std::endl;
        
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
            int[][] matrix = new int[n][n];
            for (int i = 0; i < n; i++) {
                for (int j = 0; j < n; j++) {
                    matrix[i][j] = sc.nextInt();
                }
            }
            System.out.println(solve(matrix));

            // evaluation completed
        }
        sc.close();
    }
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

        const matrix = [];
        for (let i = 0; i < n; i++) {
            const row = [];
            for (let j = 0; j < n; j++) {
                row.push(parseInt(input[idx++]));
            }
            matrix.push(row);
        }

        console.log(solve(matrix));
        // evaluation completed

    }
}


main();

## PYTHON

import math
from typing import List
from collections import deque


# user code comes here

def main():
    t = int(input())
    for _ in range(t):
        n = int(input())

        matrix = []
        for _ in range(n):
            row = list(map(int, input().split()))
            matrix.append(row)

        print(solve(matrix))
        # evaluation completed


if __name__ == "__main__":
    main()