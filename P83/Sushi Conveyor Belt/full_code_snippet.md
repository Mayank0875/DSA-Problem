## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here


int main() {
    int t;
    cin >> t;

    while (t--) {
        int n, x;
        cin >> n >> x;
        vector<int> t(n);
        for (int i = 0; i < n; ++i) {
            cin >> t[i];
        }
        cout << countSubsetsWithSum(n, x, t) << endl;
        
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
            int x = scanner.nextInt();
            int[] t = new int[n];
            for (int i = 0; i < n; i++) {
                t[i] = scanner.nextInt();
            }
            System.out.println(countSubsetsWithSum(n, x, t));

            // evaluation completed
        }
        sc.close();
    }
}
