## Title
Garden Trellis Vines

## Slug
garden-trellis-vines

## Difficulty
Medium

## Description
Two vines growing on parallel trellises need to be tied together for support.

Two parallel trellises, Trellis A and Trellis B, each contain n nodes arranged in a line.
Trellis A has an array `a` representing the height of each node.
Trellis B has an array `b` representing the height of each node.

Inside each trellis, adjacent nodes are already connected by internal stems.

You must establish inter-trellis ties connecting some nodes of Trellis A to some nodes of Trellis B.

The cost to create a tie between node i of Trellis A and node j of Trellis B is:
absolute value of (a[i] - b[j]).

**Fault-tolerance requirement:**
The final network must remain fully connected even if any single node is removed (from either Trellis A or Trellis B).
If one node fails and disappears along with all its connections, the remaining nodes must still form a single connected network.

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
It's optimal to connect four pairs of nodes:
1. node 1 from Trellis A with node 2 from Trellis B: cost |1-4| = 3.
2. node 3 from Trellis A with node 2 from Trellis B: cost |1-4| = 3.
3. node 2 from Trellis A with node 1 from Trellis B: cost |10-20| = 10.
4. node 2 from Trellis A with node 3 from Trellis B: cost |10-25| = 15.
Total cost: 3 + 3 + 10 + 15 = 31.

### 2

#### Input
4
1 1 1 1
1000000000 1000000000 1000000000 1000000000

#### Output
1999999998

#### Explanation
It is optimal to connect the first node of Trellis A with the first of Trellis B, and the last node of Trellis A with the last of Trellis B, satisfying the connectivity conditions efficiently given the values.

## Input Format
- The first line contains an integer n, the number of nodes in each trellis.
- The second line contains n integers representing the heights of Trellis A.
- The third line contains n integers representing the heights of Trellis B.

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
