## Title
Genealogy Tree Link

## Slug
genealogy-tree-link

## Difficulty
Medium

## Description
Two family branches need finding common ancestors (links) to prove relation.

Two parallel branches, Paternal Line and Maternal Line, each contain n ancestors arranged in a line.
Paternal Line has an array `a` representing the birth year of each ancestor.
Maternal Line has an array `b` representing the birth year of each ancestor.

Inside each branch, adjacent ancestors are already connected by internal descent.

You must establish inter-branch marriages connecting some ancestors of Paternal Line to some ancestors of Maternal Line.

The cost to create a marriage between ancestor i of Paternal Line and ancestor j of Maternal Line is:
absolute value of (a[i] - b[j]).

**Fault-tolerance requirement:**
The final network must remain fully connected even if any single ancestor is removed (from either Paternal Line or Maternal Line).
If one ancestor fails and disappears along with all its connections, the remaining ancestors must still form a single connected network.

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
It's optimal to connect four pairs of ancestors:
1. ancestor 1 from Paternal Line with ancestor 2 from Maternal Line: cost |1-4| = 3.
2. ancestor 3 from Paternal Line with ancestor 2 from Maternal Line: cost |1-4| = 3.
3. ancestor 2 from Paternal Line with ancestor 1 from Maternal Line: cost |10-20| = 10.
4. ancestor 2 from Paternal Line with ancestor 3 from Maternal Line: cost |10-25| = 15.
Total cost: 3 + 3 + 10 + 15 = 31.

### 2

#### Input
4
1 1 1 1
1000000000 1000000000 1000000000 1000000000

#### Output
1999999998

#### Explanation
It is optimal to connect the first ancestor of Paternal Line with the first of Maternal Line, and the last ancestor of Paternal Line with the last of Maternal Line, satisfying the connectivity conditions efficiently given the values.

## Input Format
- The first line contains an integer n, the number of ancestors in each branch.
- The second line contains n integers representing the birth years of Paternal Line.
- The third line contains n integers representing the birth years of Maternal Line.

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
