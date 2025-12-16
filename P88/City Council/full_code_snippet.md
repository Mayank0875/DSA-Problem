## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here


int main() {
    int t;
    cin >> t;

    while (t--) {
        int n; cin >> n;
        vector<int> p(n);
        for (int i = 0; i < n; i++) cin >> p[i];
        cout << solve(n, p) << endl;
        
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
            Integer[] p = new Integer[n];
            for (int i = 0; i < n; i++) {
                p[i] = sc.nextInt();
            }
            System.out.println(solve(n, p));
            // evaluation completed
        }
        sc.close();
    }
}
