## Title
Fabric Seam Stitching

## Slug
fabric-seam-stitching

## Difficulty
Medium

## Description
A tailor is stitching two pieces of fabric together. The stitch must hold even if a thread point snaps.

Two parallel fabrics, Panel A and Panel B, each contain n stitch points arranged in a line.
Panel A has an array `a` representing the fabric tension of each point.
Panel B has an array `b` representing the fabric tension of each point.

Inside each fabric, adjacent stitch points are already connected by internal weaves.

You must establish inter-fabric cross-stitches connecting some stitch points of Panel A to some stitch points of Panel B.

The cost to create a stitch between point i of Panel A and point j of Panel B is:
absolute value of (a[i] - b[j]).

**Fault-tolerance requirement:**
The final network must remain fully connected even if any single point is removed (from either Panel A or Panel B).
If one point fails and disappears along with all its connections, the remaining stitch points must still form a single connected network.

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
It's optimal to connect four pairs of stitch points:
1. point 1 from Panel A with point 2 from Panel B: cost |1-4| = 3.
2. point 3 from Panel A with point 2 from Panel B: cost |1-4| = 3.
3. point 2 from Panel A with point 1 from Panel B: cost |10-20| = 10.
4. point 2 from Panel A with point 3 from Panel B: cost |10-25| = 15.
Total cost: 3 + 3 + 10 + 15 = 31.

### 2

#### Input
4
1 1 1 1
1000000000 1000000000 1000000000 1000000000

#### Output
1999999998

#### Explanation
It is optimal to connect the first point of Panel A with the first of Panel B, and the last point of Panel A with the last of Panel B, satisfying the connectivity conditions efficiently given the values.

## Input Format
- The first line contains an integer n, the number of stitch points in each fabric.
- The second line contains n integers representing the fabric tensions of Panel A.
- The third line contains n integers representing the fabric tensions of Panel B.

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
