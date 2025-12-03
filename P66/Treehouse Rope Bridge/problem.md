## Title
Treehouse Rope Bridge

## Slug
treehouse-rope-bridge

## Difficulty
Medium

## Description
A village of treehouses in two rows of trees needs rope bridges for safe travel.

Two parallel rows, Oak Row and Pine Row, each contain n treehouses arranged in a line.
Oak Row has an array `a` representing the elevation of each treehouse.
Pine Row has an array `b` representing the elevation of each treehouse.

Inside each row, adjacent treehouses are already connected by internal ladders.

You must establish inter-row rope bridges connecting some treehouses of Oak Row to some treehouses of Pine Row.

The cost to create a bridge between treehouse i of Oak Row and treehouse j of Pine Row is:
absolute value of (a[i] - b[j]).

**Fault-tolerance requirement:**
The final network must remain fully connected even if any single treehouse is removed (from either Oak Row or Pine Row).
If one treehouse fails and disappears along with all its connections, the remaining treehouses must still form a single connected network.

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
It's optimal to connect four pairs of treehouses:
1. treehouse 1 from Oak Row with treehouse 2 from Pine Row: cost |1-4| = 3.
2. treehouse 3 from Oak Row with treehouse 2 from Pine Row: cost |1-4| = 3.
3. treehouse 2 from Oak Row with treehouse 1 from Pine Row: cost |10-20| = 10.
4. treehouse 2 from Oak Row with treehouse 3 from Pine Row: cost |10-25| = 15.
Total cost: 3 + 3 + 10 + 15 = 31.

### 2

#### Input
4
1 1 1 1
1000000000 1000000000 1000000000 1000000000

#### Output
1999999998

#### Explanation
It is optimal to connect the first treehouse of Oak Row with the first of Pine Row, and the last treehouse of Oak Row with the last of Pine Row, satisfying the connectivity conditions efficiently given the values.

## Input Format
- The first line contains an integer n, the number of treehouses in each row.
- The second line contains n integers representing the elevations of Oak Row.
- The third line contains n integers representing the elevations of Pine Row.

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
