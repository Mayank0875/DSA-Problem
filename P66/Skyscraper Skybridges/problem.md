## Title
Skyscraper Skybridges

## Slug
skyscraper-skybridges

## Difficulty
Medium

## Description
Two adjacent skyscrapers need skybridges to allow evacuation even if a floor is blocked.

Two parallel towers, Tower East and Tower West, each contain n floors arranged in a line.
Tower East has an array `a` representing the height of each floor.
Tower West has an array `b` representing the height of each floor.

Inside each tower, adjacent floors are already connected by internal stairwells.

You must establish inter-tower skybridges connecting some floors of Tower East to some floors of Tower West.

The cost to create a skybridge between floor i of Tower East and floor j of Tower West is:
absolute value of (a[i] - b[j]).

**Fault-tolerance requirement:**
The final network must remain fully connected even if any single floor is removed (from either Tower East or Tower West).
If one floor fails and disappears along with all its connections, the remaining floors must still form a single connected network.

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
It's optimal to connect four pairs of floors:
1. floor 1 from Tower East with floor 2 from Tower West: cost |1-4| = 3.
2. floor 3 from Tower East with floor 2 from Tower West: cost |1-4| = 3.
3. floor 2 from Tower East with floor 1 from Tower West: cost |10-20| = 10.
4. floor 2 from Tower East with floor 3 from Tower West: cost |10-25| = 15.
Total cost: 3 + 3 + 10 + 15 = 31.

### 2

#### Input
4
1 1 1 1
1000000000 1000000000 1000000000 1000000000

#### Output
1999999998

#### Explanation
It is optimal to connect the first floor of Tower East with the first of Tower West, and the last floor of Tower East with the last of Tower West, satisfying the connectivity conditions efficiently given the values.

## Input Format
- The first line contains an integer n, the number of floors in each tower.
- The second line contains n integers representing the heights of Tower East.
- The third line contains n integers representing the heights of Tower West.

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
