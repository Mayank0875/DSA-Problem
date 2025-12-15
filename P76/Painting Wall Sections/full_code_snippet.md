## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here


int main() {
    int t;
    cin >> t;

    while (t--) {
        int n, k; cin >> n >> k;
        vector<int> pulses(n);
        for(int i = 0; i < n; i++) cin >> pulses[i];
        cout << minTotalStress(n, k, pulses) << endl;
        
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
            int k = sc.nextInt();
            int[] pulses = new int[n];
            for (int i = 0; i < n; i++) {
                pulses[i] = sc.nextInt();
            }
            System.out.println(Solution.minTotalStress(n, k, pulses));

            // evaluation completed
        }
        sc.close();
    }
}
