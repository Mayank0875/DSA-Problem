## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here


int main() {
    int t;
    cin >> t;

    while (t--) {
        int n, m;
        cin >> n >> m;
        vector<vector<int>> teleporters(m, vector<int>(2));
        for (int i = 0; i < m; ++i) {
            cin >> teleporters[i][0] >> teleporters[i][1];
        }
        cout << maxDays(n, m, teleporters) << endl;
        
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
            int n = scanner.nextInt();
            int m = scanner.nextInt();
            int[][] teleporters = new int[m][2];
            for (int i = 0; i < m; i++) {
                teleporters[i][0] = scanner.nextInt();
                teleporters[i][1] = scanner.nextInt();
            }
            System.out.println(maxDays(n, m, teleporters));

            // evaluation completed
        }
        sc.close();
    }
}
