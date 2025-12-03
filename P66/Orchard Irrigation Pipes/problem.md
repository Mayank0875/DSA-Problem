## Title
Orchard Irrigation Pipes

## Slug
orchard-irrigation-pipes

## Difficulty
Medium

## Description
Two rows of apple trees need interconnected irrigation pipes to ensure water flow if a main line breaks.

Two parallel rows, Row 1 and Row 2, each contain n trees arranged in a line.
Row 1 has an array `a` representing the water requirement of each tree.
Row 2 has an array `b` representing the water requirement of each tree.

Inside each row, adjacent trees are already connected by internal drip lines.

You must establish inter-row connector pipes connecting some trees of Row 1 to some trees of Row 2.

The cost to create a pipe between tree i of Row 1 and tree j of Row 2 is:
absolute value of (a[i] - b[j]).

**Fault-tolerance requirement:**
The final network must remain fully connected even if any single tree is removed (from either Row 1 or Row 2).
If one tree fails and disappears along with all its connections, the remaining trees must still form a single connected network.

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
It's optimal to connect four pairs of trees:
1. tree 1 from Row 1 with tree 2 from Row 2: cost |1-4| = 3.
2. tree 3 from Row 1 with tree 2 from Row 2: cost |1-4| = 3.
3. tree 2 from Row 1 with tree 1 from Row 2: cost |10-20| = 10.
4. tree 2 from Row 1 with tree 3 from Row 2: cost |10-25| = 15.
Total cost: 3 + 3 + 10 + 15 = 31.

### 2

#### Input
4
1 1 1 1
1000000000 1000000000 1000000000 1000000000

#### Output
1999999998

#### Explanation
It is optimal to connect the first tree of Row 1 with the first of Row 2, and the last tree of Row 1 with the last of Row 2, satisfying the connectivity conditions efficiently given the values.

## Input Format
- The first line contains an integer n, the number of trees in each row.
- The second line contains n integers representing the water requirements of Row 1.
- The third line contains n integers representing the water requirements of Row 2.

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
