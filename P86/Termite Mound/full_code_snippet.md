## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here


int main() {
    int t;
    cin >> t;

    while (t--) {
        int n, m; cin >> n >> m;
        {
            vector<string> maze(n);
            for (int i = 0; i < n; ++i) {
                cin >> maze[i];
            }
            bool result = canEscape(n, m, maze);
            cout << (result ? "True" : "False") << endl;
        }
        return 0;
        
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
            int n = sc.nextInt(), m = sc.nextInt();
            char[][] maze = new char[n][m];
            for (int i = 0; i < n; i++) {
                maze[i] = sc.next().toCharArray();
            }
            System.out.println(canEscape(n, m, maze) ? "True" : "False");
        }
        sc.close();
    }
}
