## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here

int main() {
    int n, X;
    cin >> n >> X;
    vector<int> arr(n);
    for (int i = 0; i < n; i++) {
        cin >> arr[i];
    }

    long long result = OrdinaryPairs(arr, X);
    cout << result << endl;

    return 0;
}

## JAVA

import java.util.*;

public class Main {
    // user code comes here

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int X = sc.nextInt();
        int[] arr = new int[n];
        for (int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }

        System.out.println(OrdinaryPairs(arr, X));
        sc.close();
    }
}


## C

#include <stdio.h>
#include <stdlib.h>

// user code comes here

int main() {
    int n, X;
    scanf("%d %d", &n, &X);
    int arr[n];
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    printf("%lld\n", OrdinaryPairs(arr, n, X));
    return 0;
}


## JAVASCRIPT

// user code comes here

function main() {
    const fs = require("fs");
    const input = fs.readFileSync(0, "utf-8").trim().split(/\s+/);

    const n = parseInt(input[0]);
    const X = parseInt(input[1]);
    const arr = input.slice(2, 2 + n).map(Number);

    console.log(OrdinaryPairs(arr, X));
}

main();



## PYTHON

# user code comes here

def main():
    n, X = map(int, input().split())
    arr = list(map(int, input().split()))
    print(OrdinaryPairs(arr, X))

if __name__ == "__main__":
    main()
