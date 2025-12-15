## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here


int main() {
    int t;
    cin >> t;

    while (t--) {
        int n, m;
        long long k;
        cin >> n >> m >> k;
        vector<vector<int>> edges(m, vector<int>(2));
        for(int i = 0; i < m; i++) {
            cin >> edges[i][0] >> edges[i][1];
        }
        cout << countPaths(n, m, k, edges) << endl;
        
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
            long k = sc.nextLong();
            
            int[][] edges = new int[m][2];
            for (int i = 0; i < m; i++) {
                edges[i][0] = sc.nextInt();
                edges[i][1] = sc.nextInt();
            }
            
            System.out.println(countPaths(n, m, k, edges));
            // evaluation completed
        }
        sc.close();
    }
}
