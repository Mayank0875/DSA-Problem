## Title
Library Shelf Bracing

## Slug
library-shelf-bracing

## Difficulty
Medium

## Description
Two tall library shelves need metal braces connecting them to prevent collapse if a shelf fails.

Two parallel shelves, Fiction and Non-Fiction, each contain n levels arranged in a line.
Fiction has an array `a` representing the load weight of each level.
Non-Fiction has an array `b` representing the load weight of each level.

Inside each shelf, adjacent levels are already connected by internal frames.

You must establish inter-shelf cross-braces connecting some levels of Fiction to some levels of Non-Fiction.

The cost to create a brace between level i of Fiction and level j of Non-Fiction is:
absolute value of (a[i] - b[j]).

**Fault-tolerance requirement:**
The final network must remain fully connected even if any single level is removed (from either Fiction or Non-Fiction).
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
1. level 1 from Fiction with level 2 from Non-Fiction: cost |1-4| = 3.
2. level 3 from Fiction with level 2 from Non-Fiction: cost |1-4| = 3.
3. level 2 from Fiction with level 1 from Non-Fiction: cost |10-20| = 10.
4. level 2 from Fiction with level 3 from Non-Fiction: cost |10-25| = 15.
Total cost: 3 + 3 + 10 + 15 = 31.

### 2

#### Input
4
1 1 1 1
1000000000 1000000000 1000000000 1000000000

#### Output
1999999998

#### Explanation
It is optimal to connect the first level of Fiction with the first of Non-Fiction, and the last level of Fiction with the last of Non-Fiction, satisfying the connectivity conditions efficiently given the values.

## Input Format
- The first line contains an integer n, the number of levels in each shelf.
- The second line contains n integers representing the load weights of Fiction.
- The third line contains n integers representing the load weights of Non-Fiction.

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
