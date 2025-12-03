## Title
Highway Emergency U-Turns

## Slug
highway-emergency-u-turns

## Difficulty
Medium

## Description
Two sides of a highway need emergency turnaround points to divert traffic during accidents.

Two parallel highways, Northbound and Southbound, each contain n mile markers arranged in a line.
Northbound has an array `a` representing the traffic density of each marker.
Southbound has an array `b` representing the traffic density of each marker.

Inside each highway, adjacent mile markers are already connected by internal lanes.

You must establish inter-highway U-turn lanes connecting some mile markers of Northbound to some mile markers of Southbound.

The cost to create a lane between marker i of Northbound and marker j of Southbound is:
absolute value of (a[i] - b[j]).

**Fault-tolerance requirement:**
The final network must remain fully connected even if any single marker is removed (from either Northbound or Southbound).
If one marker fails and disappears along with all its connections, the remaining mile markers must still form a single connected network.

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
It's optimal to connect four pairs of mile markers:
1. marker 1 from Northbound with marker 2 from Southbound: cost |1-4| = 3.
2. marker 3 from Northbound with marker 2 from Southbound: cost |1-4| = 3.
3. marker 2 from Northbound with marker 1 from Southbound: cost |10-20| = 10.
4. marker 2 from Northbound with marker 3 from Southbound: cost |10-25| = 15.
Total cost: 3 + 3 + 10 + 15 = 31.

### 2

#### Input
4
1 1 1 1
1000000000 1000000000 1000000000 1000000000

#### Output
1999999998

#### Explanation
It is optimal to connect the first marker of Northbound with the first of Southbound, and the last marker of Northbound with the last of Southbound, satisfying the connectivity conditions efficiently given the values.

## Input Format
- The first line contains an integer n, the number of mile markers in each highway.
- The second line contains n integers representing the traffic densitys of Northbound.
- The third line contains n integers representing the traffic densitys of Southbound.

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
