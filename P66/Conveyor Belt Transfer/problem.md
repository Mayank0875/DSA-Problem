## Title
Conveyor Belt Transfer

## Slug
conveyor-belt-transfer

## Difficulty
Medium

## Description
Two factory conveyor belts need transfer arms to reroute items if a motor fails.

Two parallel belts, Assembly Belt and Packaging Belt, each contain n stations arranged in a line.
Assembly Belt has an array `a` representing the belt speed of each station.
Packaging Belt has an array `b` representing the belt speed of each station.

Inside each belt, adjacent stations are already connected by internal rollers.

You must establish inter-belt transfer arms connecting some stations of Assembly Belt to some stations of Packaging Belt.

The cost to create a arm between station i of Assembly Belt and station j of Packaging Belt is:
absolute value of (a[i] - b[j]).

**Fault-tolerance requirement:**
The final network must remain fully connected even if any single station is removed (from either Assembly Belt or Packaging Belt).
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
1. station 1 from Assembly Belt with station 2 from Packaging Belt: cost |1-4| = 3.
2. station 3 from Assembly Belt with station 2 from Packaging Belt: cost |1-4| = 3.
3. station 2 from Assembly Belt with station 1 from Packaging Belt: cost |10-20| = 10.
4. station 2 from Assembly Belt with station 3 from Packaging Belt: cost |10-25| = 15.
Total cost: 3 + 3 + 10 + 15 = 31.

### 2

#### Input
4
1 1 1 1
1000000000 1000000000 1000000000 1000000000

#### Output
1999999998

#### Explanation
It is optimal to connect the first station of Assembly Belt with the first of Packaging Belt, and the last station of Assembly Belt with the last of Packaging Belt, satisfying the connectivity conditions efficiently given the values.

## Input Format
- The first line contains an integer n, the number of stations in each belt.
- The second line contains n integers representing the belt speeds of Assembly Belt.
- The third line contains n integers representing the belt speeds of Packaging Belt.

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
