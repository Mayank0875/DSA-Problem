## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here

int main() {
    int t;
    cin >> t;
    while(t--){
        long long l, r;
        cin >> l >> r;

        long long result = countPerfectSquaresInRange(arr, target);
        cout << result << endl;
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
            long l = sc.nextLong();
            long r = sc.nextLong();

            long result = countPerfectSquaresInRange(l, r);
            System.out.println(result);
        }
        sc.close();
    }
}

## C

#include <stdio.h>

// user code comes here

int main() {
    int t;
    scanf("%d", &t);
    while (t--) {
        long long l, r;
        scanf("%lld %lld", &l, &r);

        long long result = countPerfectSquaresInRange(l, r);
        printf("%lld\n", result);
    }
    return 0;
}

## JAVASCRIPT

// user code comes here

// user code comes here

function main() {
    const fs = require("fs");
    const input = fs.readFileSync(0, "utf-8").trim().split(/\s+/).map(Number);

    let idx = 0;
    const t = input[idx++];

    for (let test = 0; test < t; test++) {
        const l = input[idx++];
        const r = input[idx++];

        const result = countPerfectSquaresInRange(l, r);
        console.log(result);
    }
}

main();

## PYTHON


# user code comes here

def main():
    t = int(input())
    for _ in range(t):
        l, r = map(int, input().split())
        result = countPerfectSquaresInRange(l, r)
        print(result)

if __name__ == "__main__":
    main()
