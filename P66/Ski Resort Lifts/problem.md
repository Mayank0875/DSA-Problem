## Title
Ski Resort Lifts

## Slug
ski-resort-lifts

## Difficulty
Medium

## Description
Two parallel ski runs need connector lifts so skiers aren't stranded if a run closes.

Two parallel runs, Green Run and Blue Run, each contain n stations arranged in a line.
Green Run has an array `a` representing the elevation of each station.
Blue Run has an array `b` representing the elevation of each station.

Inside each run, adjacent stations are already connected by internal slopes.

You must establish inter-run connector lifts connecting some stations of Green Run to some stations of Blue Run.

The cost to create a lift between station i of Green Run and station j of Blue Run is:
absolute value of (a[i] - b[j]).

**Fault-tolerance requirement:**
The final network must remain fully connected even if any single station is removed (from either Green Run or Blue Run).
If one station fails and disappears along with all its connections, the remaining stations must still form a single connected network.

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
It's optimal to connect four pairs of stations:
1. station 1 from Green Run with station 2 from Blue Run: cost |1-4| = 3.
2. station 3 from Green Run with station 2 from Blue Run: cost |1-4| = 3.
3. station 2 from Green Run with station 1 from Blue Run: cost |10-20| = 10.
4. station 2 from Green Run with station 3 from Blue Run: cost |10-25| = 15.
Total cost: 3 + 3 + 10 + 15 = 31.

### 2

#### Input
4
1 1 1 1
1000000000 1000000000 1000000000 1000000000

#### Output
1999999998

#### Explanation
It is optimal to connect the first station of Green Run with the first of Blue Run, and the last station of Green Run with the last of Blue Run, satisfying the connectivity conditions efficiently given the values.

## Input Format
- The first line contains an integer n, the number of stations in each run.
- The second line contains n integers representing the elevations of Green Run.
- The third line contains n integers representing the elevations of Blue Run.

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
