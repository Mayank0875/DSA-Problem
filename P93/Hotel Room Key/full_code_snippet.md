## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here


int main() {
    int t;
    cin >> t;

    while (t--) {
        string K; int D;
        cin >> K >> D;
        cout << countAccessCodes(K, D) << endl;
        
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
            String K = scanner.next();
            int D = scanner.nextInt();
            System.out.println(countAccessCodes(K, D));
            // evaluation completed
        }
        sc.close();
    }
}

