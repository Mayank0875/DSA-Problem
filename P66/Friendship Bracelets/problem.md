## Title
Friendship Bracelets

## Slug
friendship-bracelets

## Difficulty
Medium

## Description
Two strands of a bracelet are tied together at intervals to prevent unraveling.

Two parallel strands, Blue Strand and Red Strand, each contain n beads arranged in a line.
Blue Strand has an array `a` representing the color code of each bead.
Red Strand has an array `b` representing the color code of each bead.

Inside each strand, adjacent beads are already connected by internal strings.

You must establish inter-strand knots connecting some beads of Blue Strand to some beads of Red Strand.

The cost to create a knot between bead i of Blue Strand and bead j of Red Strand is:
absolute value of (a[i] - b[j]).

**Fault-tolerance requirement:**
The final network must remain fully connected even if any single bead is removed (from either Blue Strand or Red Strand).
If one bead fails and disappears along with all its connections, the remaining beads must still form a single connected network.

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
It's optimal to connect four pairs of beads:
1. bead 1 from Blue Strand with bead 2 from Red Strand: cost |1-4| = 3.
2. bead 3 from Blue Strand with bead 2 from Red Strand: cost |1-4| = 3.
3. bead 2 from Blue Strand with bead 1 from Red Strand: cost |10-20| = 10.
4. bead 2 from Blue Strand with bead 3 from Red Strand: cost |10-25| = 15.
Total cost: 3 + 3 + 10 + 15 = 31.

### 2

#### Input
4
1 1 1 1
1000000000 1000000000 1000000000 1000000000

#### Output
1999999998

#### Explanation
It is optimal to connect the first bead of Blue Strand with the first of Red Strand, and the last bead of Blue Strand with the last of Red Strand, satisfying the connectivity conditions efficiently given the values.

## Input Format
- The first line contains an integer n, the number of beads in each strand.
- The second line contains n integers representing the color codes of Blue Strand.
- The third line contains n integers representing the color codes of Red Strand.

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
