## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here


int main() {
    int t;
    cin >> t;

    while (t--) {
        int n, m, k;
        cin >> n >> m >> k;
        vector<pair<int, int>> pairs(k);
        for (int i = 0; i < k; i++) {
            cin >> pairs[i].first >> pairs[i].second;
        }
        cout << solve(n, m, pairs) << endl;
        
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
            int k = sc.nextInt();
            int[][] pairs = new int[k][2];
            for (int i = 0; i < k; i++) {
                pairs[i][0] = sc.nextInt();
                pairs[i][1] = sc.nextInt();
            }
            System.out.println(solve(n, m, pairs));

            // evaluation completed
        }
        sc.close();
    }
}
