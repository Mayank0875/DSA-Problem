## Title
Canal Lock Gates

## Slug
canal-lock-gates

## Difficulty
Medium

## Description
Two parallel canals need interconnecting sluice gates to manage water levels during maintenance.

Two parallel canals, Canal East and Canal West, each contain n locks arranged in a line.
Canal East has an array `a` representing the water level of each lock.
Canal West has an array `b` representing the water level of each lock.

Inside each canal, adjacent locks are already connected by internal channels.

You must establish inter-canal sluice pipes connecting some locks of Canal East to some locks of Canal West.

The cost to create a pipe between lock i of Canal East and lock j of Canal West is:
absolute value of (a[i] - b[j]).

**Fault-tolerance requirement:**
The final network must remain fully connected even if any single lock is removed (from either Canal East or Canal West).
If one lock fails and disappears along with all its connections, the remaining locks must still form a single connected network.

Your task is to calculate the minimum total cost required to build such a set of connections.

## Examples

### 1

#### Input
3
1 10 1
20 4 25

#### Output
31

#### Explanation
It's optimal to connect four pairs of locks:
1. lock 1 from Canal East with lock 2 from Canal West: cost |1-4| = 3.
2. lock 3 from Canal East with lock 2 from Canal West: cost |1-4| = 3.
3. lock 2 from Canal East with lock 1 from Canal West: cost |10-20| = 10.
4. lock 2 from Canal East with lock 3 from Canal West: cost |10-25| = 15.
Total cost: 3 + 3 + 10 + 15 = 31.

### 2

#### Input
4
1 1 1 1
1000000000 1000000000 1000000000 1000000000

#### Output
1999999998

#### Explanation
It is optimal to connect the first lock of Canal East with the first of Canal West, and the last lock of Canal East with the last of Canal West, satisfying the connectivity conditions efficiently given the values.

## Input Format
- The first line contains an integer n, the number of locks in each canal.
- The second line contains n integers representing the water levels of Canal East.
- The third line contains n integers representing the water levels of Canal West.

## Output Format
- Return a single integer representing the minimum total cost to make the network fault-tolerant.

## Constraints
- 3 ≤ n ≤ 10^5
- 1 ≤ a[i], b[i] ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, greedy, math
