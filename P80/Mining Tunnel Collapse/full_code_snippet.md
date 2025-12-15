## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here


int main() {
    int t;
    cin >> t;

    while (t--) {
        int n, m; cin >> n >> m;
        vector<vector<int>> streets(m, vector<int>(2));
        for (int i = 0; i < m; ++i) {
            cin >> streets[i][0] >> streets[i][1];
        }
        cout << minStreets(n, m, streets) << endl;
        
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
            int[][] streets = new int[m][2];
            for (int i = 0; i < m; i++) {
                streets[i][0] = scanner.nextInt();
                streets[i][1] = scanner.nextInt();
            }
            System.out.println(minStreets(n, m, streets));
            // evaluation completed
        }
        sc.close();
    }
}
