## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here

int main() {
    int t; cin >> t;
    while (t--) {
        int n; cin >> n;
        vector<vector<int>> tree(n - 1, vector<int>(2, 0));

        for (int i = 0; i < n - 1; ++i) {
            cin >> tree[i][0] >> tree[i][1];
        }

        cout << Mininum_Edges(tree) << endl;
        // evaluation completed
    }
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
            List<List<Integer>> tree = new ArrayList<>();
            for (int i = 0; i < n - 1; i++) {
                int u = sc.nextInt();
                int v = sc.nextInt();
                tree.add(Arrays.asList(u, v));
            }

            System.out.println(Mininum_Edges(tree));
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
        int n;
        scanf("%d", &n);
        int** tree = (int**)malloc((n - 1) * sizeof(int*));
        for (int i = 0; i < n - 1; i++) {
            tree[i] = (int*)malloc(2 * sizeof(int));
            scanf("%d %d", &tree[i][0], &tree[i][1]);
        }

        printf("%d\n", Mininum_Edges(tree, n - 1));

        for (int i = 0; i < n - 1; i++) {
            free(tree[i]);
        }
        free(tree);
        // evaluation completed
    }
    return 0;
}

## JAVASCRIPT

// user code comes here

const fs = require("fs");
const data = fs.readFileSync(0, "utf8").trim().split(/\s+/);
let idx = 0, t = +data[idx++];
while (t--) {
    const n = +data[idx++];
    const tree = [];
    for (let i = 0; i < n - 1; i++) {
        const u = +data[idx++];
        const v = +data[idx++];
        tree.push([u, v]);
    }

    console.log(Mininum_Edges(tree));
    // evaluation completed
}

## PYTHON

from collections import deque

# user code comes here

t = int(input().strip())
for _ in range(t):
    n = int(input().strip())
    tree = []
    for _ in range(n - 1):
        u, v = map(int, input().strip().split())
        tree.append((u, v))

    print(Mininum_Edges(tree))
    # evaluation completed