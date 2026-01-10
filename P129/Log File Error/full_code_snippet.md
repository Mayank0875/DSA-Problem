## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here


int main() {
    int t;
    cin >> t;

    while (t--) {
        string s, t;
        if (cin >> s >> t) {
            cout << countSubsequences(s, t) << endl;
        }
        
        // evaluation completed
    }
    return 0;
}

## JAVA

import java.util.*;

public class Main {

    // user code comes here
    // static long countSubsequences(String s, String t) { }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int tc = sc.nextInt();

        while (tc-- > 0) {
            String s = sc.next();
            String t = sc.next();

            System.out.println(countSubsequences(s, t));
            // evaluation completed
        }
        sc.close();
    }
}

## C

#include <stdio.h>

// user code comes here

int main() {
    int tc;
    scanf("%d", &tc);

    while (tc--) {
        char s[100005];
        char t[100005];

        scanf("%s %s", s, t);
        printf("%lld\n", countSubsequences(s, t));
        // evaluation completed
    }
    return 0;
}


## JAVASCRIPT

// user code comes here

function main() {
    const fs = require("fs");
    const input = fs.readFileSync(0, "utf-8").trim().split(/\s+/);
    let idx = 0;

    const tc = Number(input[idx++]);
    for (let i = 0; i < tc; i++) {
        const s = input[idx++];
        const t = input[idx++];

        console.log(countSubsequences(s, t));
        // evaluation completed
    }
}

main();


## PYTHON

# user code comes here

def main():
    tc = int(input())
    for _ in range(tc):
        s, t = input().split()
        print(countSubsequences(s, t))
        # evaluation completed

if __name__ == "__main__":
    main()
