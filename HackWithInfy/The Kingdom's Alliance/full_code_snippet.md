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

        cout << maxMatching(n, tree) << endl;
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

            System.out.println(maxMatching(n, tree));
            // evaluation completed
        }
        sc.close();
    }
}