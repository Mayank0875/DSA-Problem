## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here


int main() {
    int t;
    cin >> t;

    while (t--) {
        int n, m;
        if (cin >> n >> m) {
            vector<long long> cities(n);
            for(int i=0; i<n; ++i) cin >> cities[i];
            
            vector<long long> towers(m);
            for(int i=0; i<m; ++i) cin >> towers[i];
            
            sort(cities.begin(), cities.end());
            sort(towers.begin(), towers.end());

            cout << minRadius(n, m, cities, towers) << endl;
        }
        
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
            int m = sc.nextInt();

            long[] cities = new long[n];
            for (int i = 0; i < n; i++) cities[i] = sc.nextLong();

            long[] towers = new long[m];
            for (int i = 0; i < m; i++) towers[i] = sc.nextLong();

            Arrays.sort(cities);
            Arrays.sort(towers);

            System.out.println(minRadius(n, m, cities, towers));
            // evaluation completed
        }
        sc.close();
    }
}


## C

#include <stdio.h>
#include <stdlib.h>

// user code comes here

int cmp(const void* a, const void* b) {
    long long x = *(long long*)a;
    long long y = *(long long*)b;
    return (x > y) - (x < y);
}

int main() {
    int t;
    scanf("%d", &t);

    while (t--) {
        int n, m;
        scanf("%d %d", &n, &m);

        long long cities[n];
        for (int i = 0; i < n; i++) scanf("%lld", &cities[i]);

        long long towers[m];
        for (int i = 0; i < m; i++) scanf("%lld", &towers[i]);

        qsort(cities, n, sizeof(long long), cmp);
        qsort(towers, m, sizeof(long long), cmp);

        printf("%lld\n", minRadius(n, m, cities, towers));
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

    const t = Number(input[idx++]);

    for (let tc = 0; tc < t; tc++) {
        const n = Number(input[idx++]);
        const m = Number(input[idx++]);

        const cities = [];
        for (let i = 0; i < n; i++) cities.push(BigInt(input[idx++]));

        const towers = [];
        for (let i = 0; i < m; i++) towers.push(BigInt(input[idx++]));

        cities.sort((a, b) => (a < b ? -1 : 1));
        towers.sort((a, b) => (a < b ? -1 : 1));

        console.log(minRadius(n, m, cities, towers).toString());
        // evaluation completed
    }
}

main();


## PYTHON

from typing import List

# user code comes here

def main():
    t = int(input())
    for _ in range(t):
        n, m = map(int, input().split())
        cities = list(map(int, input().split()))
        towers = list(map(int, input().split()))

        cities.sort()
        towers.sort()

        print(minRadius(n, m, cities, towers))
        # evaluation completed

if __name__ == "__main__":
    main()
