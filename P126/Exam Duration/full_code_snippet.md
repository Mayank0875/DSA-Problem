## CPP

#include <bits/stdc++.h>
using namespace std;

// user code comes here


int main() {
    int t;
    cin >> t;

    while (t--) {
        int n;
        if (!(cin >> n)) return 0;
        
        vector<int> startTime(n);
        for(int i = 0; i < n; i++) cin >> startTime[i];
        
        vector<int> endTime(n);
        for(int i = 0; i < n; i++) cin >> endTime[i];
        
        int qStart, qEnd;
        cin >> qStart >> qEnd;
        
        cout << countStudents(startTime, endTime, qStart, qEnd) << endl;
        
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

            int[] startTime = new int[n];
            for (int i = 0; i < n; i++) startTime[i] = sc.nextInt();

            int[] endTime = new int[n];
            for (int i = 0; i < n; i++) endTime[i] = sc.nextInt();

            int qStart = sc.nextInt();
            int qEnd = sc.nextInt();

            System.out.println(countStudents(startTime, endTime, qStart, qEnd));
            // evaluation completed
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
        int n;
        scanf("%d", &n);

        int startTime[n];
        for (int i = 0; i < n; i++) scanf("%d", &startTime[i]);

        int endTime[n];
        for (int i = 0; i < n; i++) scanf("%d", &endTime[i]);

        int qStart, qEnd;
        scanf("%d %d", &qStart, &qEnd);

        printf("%d\n",
            countStudents(startTime, n, endTime, n, qStart, qEnd));
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

        const startTime = [];
        for (let i = 0; i < n; i++) startTime.push(Number(input[idx++]));

        const endTime = [];
        for (let i = 0; i < n; i++) endTime.push(Number(input[idx++]));

        const qStart = Number(input[idx++]);
        const qEnd = Number(input[idx++]);

        console.log(countStudents(startTime, endTime, qStart, qEnd));
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
        n = int(input())
        startTime = list(map(int, input().split()))
        endTime = list(map(int, input().split()))
        qStart, qEnd = map(int, input().split())

        print(countStudents(startTime, endTime, qStart, qEnd))
        # evaluation completed

if __name__ == "__main__":
    main()
