## Title
Climbing Ladder Safety

## Slug
climbing-ladder-safety

## Difficulty
Medium

## Description
Two parallel ladders on a cliff need connecting ropes so climbers can switch if a rung breaks.

Two parallel ladders, Route A and Route B, each contain n anchors arranged in a line.
Route A has an array `a` representing the rock quality of each anchor.
Route B has an array `b` representing the rock quality of each anchor.

Inside each ladder, adjacent anchors are already connected by internal rungs.

You must establish inter-ladder safety ropes connecting some anchors of Route A to some anchors of Route B.

The cost to create a rope between anchor i of Route A and anchor j of Route B is:
absolute value of (a[i] - b[j]).

**Fault-tolerance requirement:**
The final network must remain fully connected even if any single anchor is removed (from either Route A or Route B).
If one anchor fails and disappears along with all its connections, the remaining anchors must still form a single connected network.

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
It's optimal to connect four pairs of anchors:
1. anchor 1 from Route A with anchor 2 from Route B: cost |1-4| = 3.
2. anchor 3 from Route A with anchor 2 from Route B: cost |1-4| = 3.
3. anchor 2 from Route A with anchor 1 from Route B: cost |10-20| = 10.
4. anchor 2 from Route A with anchor 3 from Route B: cost |10-25| = 15.
Total cost: 3 + 3 + 10 + 15 = 31.

### 2

#### Input
4
1 1 1 1
1000000000 1000000000 1000000000 1000000000

#### Output
1999999998

#### Explanation
It is optimal to connect the first anchor of Route A with the first of Route B, and the last anchor of Route A with the last of Route B, satisfying the connectivity conditions efficiently given the values.

## Input Format
- The first line contains an integer n, the number of anchors in each ladder.
- The second line contains n integers representing the rock qualitys of Route A.
- The third line contains n integers representing the rock qualitys of Route B.

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
