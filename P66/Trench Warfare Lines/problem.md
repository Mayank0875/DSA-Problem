## Title
Trench Warfare Lines

## Slug
trench-warfare-lines

## Difficulty
Medium

## Description
Military engineers are securing supply lines between two parallel trenches.

Two parallel trenches, Front Line and Support Line, each contain n bunkers arranged in a line.
Front Line has an array `a` representing the strategic value of each bunker.
Support Line has an array `b` representing the strategic value of each bunker.

Inside each trench, adjacent bunkers are already connected by internal tunnels.

You must establish inter-trench supply paths connecting some bunkers of Front Line to some bunkers of Support Line.

The cost to create a path between bunker i of Front Line and bunker j of Support Line is:
absolute value of (a[i] - b[j]).

**Fault-tolerance requirement:**
The final network must remain fully connected even if any single bunker is removed (from either Front Line or Support Line).
If one bunker fails and disappears along with all its connections, the remaining bunkers must still form a single connected network.

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
It's optimal to connect four pairs of bunkers:
1. bunker 1 from Front Line with bunker 2 from Support Line: cost |1-4| = 3.
2. bunker 3 from Front Line with bunker 2 from Support Line: cost |1-4| = 3.
3. bunker 2 from Front Line with bunker 1 from Support Line: cost |10-20| = 10.
4. bunker 2 from Front Line with bunker 3 from Support Line: cost |10-25| = 15.
Total cost: 3 + 3 + 10 + 15 = 31.

### 2

#### Input
4
1 1 1 1
1000000000 1000000000 1000000000 1000000000

#### Output
1999999998

#### Explanation
It is optimal to connect the first bunker of Front Line with the first of Support Line, and the last bunker of Front Line with the last of Support Line, satisfying the connectivity conditions efficiently given the values.

## Input Format
- The first line contains an integer n, the number of bunkers in each trench.
- The second line contains n integers representing the strategic values of Front Line.
- The third line contains n integers representing the strategic values of Support Line.

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
