## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here


int main() {
    int t;
    cin >> t;

    while (t--) {
        int n;
        cin >> n;
        std::vector<int> arr(n);
        for(int i = 0; i < n; ++i) {
            std::cin >> arr[i];
        }
        std::cout << solveQuantumSignal(n, arr) << std::endl;
        
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
            int[] arr = new int[n];
            for(int i = 0; i < n; i++) {
                arr[i] = scanner.nextInt();
            }
            System.out.println(solveQuantumSignal(n, arr));
            // evaluation completed
        }
        sc.close();
    }
}
