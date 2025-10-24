## CPP

#include <bits/stdc++.h>
using namespace std;

// User function to implement


int main() {
    int t;
    cin >> t;

    while (t--) {
        string s;
        cin >> s;
        cout << isPalindrome(s) << "\n";
        
        // evaluation completed
    }
    return 0;
}

## JAVA

import java.util.*;

public class Main {
    // User function to implement
    
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int t = sc.nextInt();
        while (t-- > 0) {
            String s = sc.next();
            System.out.println(isPalindrome(s));
            // evaluation completed
        }
        sc.close();
    }
}

## C

#include <stdio.h>
#include <string.h>

// User function to implement

int main() {
    int t;
    scanf("%d", &t);
    while (t--) {
        char s[100000];
        scanf("%s", s);
        printf("%s\n", isPalindrome(s));
        // evaluation completed
    }
    return 0;
}

## JAVASCRIPT

// User function to implement

function main() {
    const fs = require("fs");
    const input = fs.readFileSync(0, "utf-8").trim().split(/\s+/);
    let idx = 0;

    const t = parseInt(input[idx++]);
    for (let tc = 0; tc < t; tc++) {
        const s = input[idx++];
        console.log(isPalindrome(s));
        // evaluation completed
    }
}

main();

## PYTHON

# User function to implement

def main():
    t = int(input())
    for _ in range(t):
        s = input().strip()
        print(isPalindrome(s))
        
        # evaluation completed

if __name__ == "__main__":
    main()