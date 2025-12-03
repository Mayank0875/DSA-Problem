## Title
Apartment Balcony Walkway

## Slug
apartment-balcony-walkway

## Difficulty
Medium

## Description
Two apartment blocks face each other. Architects want to build walkways connecting balconies.

Two parallel blocks, Block East and Block West, each contain n apartments arranged in a line.
Block East has an array `a` representing the floor number of each apartment.
Block West has an array `b` representing the floor number of each apartment.

Inside each block, adjacent apartments are already connected by internal corridors.

You must establish inter-block balcony bridges connecting some apartments of Block East to some apartments of Block West.

The cost to create a bridge between apartment i of Block East and apartment j of Block West is:
absolute value of (a[i] - b[j]).

**Fault-tolerance requirement:**
The final network must remain fully connected even if any single apartment is removed (from either Block East or Block West).
If one apartment fails and disappears along with all its connections, the remaining apartments must still form a single connected network.

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
It's optimal to connect four pairs of apartments:
1. apartment 1 from Block East with apartment 2 from Block West: cost |1-4| = 3.
2. apartment 3 from Block East with apartment 2 from Block West: cost |1-4| = 3.
3. apartment 2 from Block East with apartment 1 from Block West: cost |10-20| = 10.
4. apartment 2 from Block East with apartment 3 from Block West: cost |10-25| = 15.
Total cost: 3 + 3 + 10 + 15 = 31.

### 2

#### Input
4
1 1 1 1
1000000000 1000000000 1000000000 1000000000

#### Output
1999999998

#### Explanation
It is optimal to connect the first apartment of Block East with the first of Block West, and the last apartment of Block East with the last of Block West, satisfying the connectivity conditions efficiently given the values.

## Input Format
- The first line contains an integer n, the number of apartments in each block.
- The second line contains n integers representing the floor numbers of Block East.
- The third line contains n integers representing the floor numbers of Block West.

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
