## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here


int main() {
    int t;
    cin >> t;

    while (t--) {
        int n; cin >> n;
        vector<vector<int>> arr(n, vector<int>(2, 0));

        for(int i = 0; i < n; ++i){
            cin >> arr[i][0] >> arr[i][1];
        }

        cout << minTransmissionCost(n, arr) << endl;
        
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
            long[][] arr = new long[n][2];

            for (int i = 0; i < n; ++i) {
                arr[i][0] = sc.nextLong();
                arr[i][1] = sc.nextLong();
            }

            System.out.println(minTransmissionCost(n, arr));
            // evaluation completed
        }

        sc.close();
    }
}
