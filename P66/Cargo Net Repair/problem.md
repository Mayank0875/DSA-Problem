## Title
Cargo Net Repair

## Slug
cargo-net-repair

## Difficulty
Medium

## Description
A cargo net made of two main ropes needs cross-weaving to hold heavy loads.

Two parallel ropes, Rope 1 and Rope 2, each contain n knots arranged in a line.
Rope 1 has an array `a` representing the tensile strength of each knot.
Rope 2 has an array `b` representing the tensile strength of each knot.

Inside each rope, adjacent knots are already connected by internal twine.

You must establish inter-rope weaves connecting some knots of Rope 1 to some knots of Rope 2.

The cost to create a weave between knot i of Rope 1 and knot j of Rope 2 is:
absolute value of (a[i] - b[j]).

**Fault-tolerance requirement:**
The final network must remain fully connected even if any single knot is removed (from either Rope 1 or Rope 2).
If one knot fails and disappears along with all its connections, the remaining knots must still form a single connected network.

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
It's optimal to connect four pairs of knots:
1. knot 1 from Rope 1 with knot 2 from Rope 2: cost |1-4| = 3.
2. knot 3 from Rope 1 with knot 2 from Rope 2: cost |1-4| = 3.
3. knot 2 from Rope 1 with knot 1 from Rope 2: cost |10-20| = 10.
4. knot 2 from Rope 1 with knot 3 from Rope 2: cost |10-25| = 15.
Total cost: 3 + 3 + 10 + 15 = 31.

### 2

#### Input
4
1 1 1 1
1000000000 1000000000 1000000000 1000000000

#### Output
1999999998

#### Explanation
It is optimal to connect the first knot of Rope 1 with the first of Rope 2, and the last knot of Rope 1 with the last of Rope 2, satisfying the connectivity conditions efficiently given the values.

## Input Format
- The first line contains an integer n, the number of knots in each rope.
- The second line contains n integers representing the tensile strengths of Rope 1.
- The third line contains n integers representing the tensile strengths of Rope 2.

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
