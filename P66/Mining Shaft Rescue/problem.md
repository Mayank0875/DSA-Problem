## Title
Mining Shaft Rescue

## Slug
mining-shaft-rescue

## Difficulty
Medium

## Description
Two vertical mining shafts need horizontal rescue tunnels to ensure miners can escape a collapse.

Two parallel shafts, Shaft 1 and Shaft 2, each contain n levels arranged in a line.
Shaft 1 has an array `a` representing the depth of each level.
Shaft 2 has an array `b` representing the depth of each level.

Inside each shaft, adjacent levels are already connected by internal elevators.

You must establish inter-shaft rescue tunnels connecting some levels of Shaft 1 to some levels of Shaft 2.

The cost to create a tunnel between level i of Shaft 1 and level j of Shaft 2 is:
absolute value of (a[i] - b[j]).

**Fault-tolerance requirement:**
The final network must remain fully connected even if any single level is removed (from either Shaft 1 or Shaft 2).
If one level fails and disappears along with all its connections, the remaining levels must still form a single connected network.

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
It's optimal to connect four pairs of levels:
1. level 1 from Shaft 1 with level 2 from Shaft 2: cost |1-4| = 3.
2. level 3 from Shaft 1 with level 2 from Shaft 2: cost |1-4| = 3.
3. level 2 from Shaft 1 with level 1 from Shaft 2: cost |10-20| = 10.
4. level 2 from Shaft 1 with level 3 from Shaft 2: cost |10-25| = 15.
Total cost: 3 + 3 + 10 + 15 = 31.

### 2

#### Input
4
1 1 1 1
1000000000 1000000000 1000000000 1000000000

#### Output
1999999998

#### Explanation
It is optimal to connect the first level of Shaft 1 with the first of Shaft 2, and the last level of Shaft 1 with the last of Shaft 2, satisfying the connectivity conditions efficiently given the values.

## Input Format
- The first line contains an integer n, the number of levels in each shaft.
- The second line contains n integers representing the depths of Shaft 1.
- The third line contains n integers representing the depths of Shaft 2.

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
