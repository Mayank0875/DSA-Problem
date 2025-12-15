## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here


int main() {
    int t;
    cin >> t;

    while (t--) {
        int n;cin >> n;
        vector<int> x(n);
        for(int i = 0; i < n; i++) {
            cin >> x[i];
        }
        cout << solve(n, x) << endl;

        
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
            int[] x = new int[n];
            for (int i = 0; i < n; i++) {
                x[i] = scanner.nextInt();
            }
            System.out.println(solve(n, x));
            // evaluation completed
        }
        sc.close();
    }
}
