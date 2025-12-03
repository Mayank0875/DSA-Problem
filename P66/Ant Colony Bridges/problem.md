## Title
Ant Colony Bridges

## Slug
ant-colony-bridges

## Difficulty
Medium

## Description
Ants are building bridges between two parallel leaves to secure their path against wind.

Two parallel leaves, Leaf Left and Leaf Right, each contain n anchor points arranged in a line.
Leaf Left has an array `a` representing the surface texture of each point.
Leaf Right has an array `b` representing the surface texture of each point.

Inside each leaf, adjacent anchor points are already connected by internal leaf veins.

You must establish inter-leaf ant bridges connecting some anchor points of Leaf Left to some anchor points of Leaf Right.

The cost to create a bridge between point i of Leaf Left and point j of Leaf Right is:
absolute value of (a[i] - b[j]).

**Fault-tolerance requirement:**
The final network must remain fully connected even if any single point is removed (from either Leaf Left or Leaf Right).
If one point fails and disappears along with all its connections, the remaining anchor points must still form a single connected network.

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
It's optimal to connect four pairs of anchor points:
1. point 1 from Leaf Left with point 2 from Leaf Right: cost |1-4| = 3.
2. point 3 from Leaf Left with point 2 from Leaf Right: cost |1-4| = 3.
3. point 2 from Leaf Left with point 1 from Leaf Right: cost |10-20| = 10.
4. point 2 from Leaf Left with point 3 from Leaf Right: cost |10-25| = 15.
Total cost: 3 + 3 + 10 + 15 = 31.

### 2

#### Input
4
1 1 1 1
1000000000 1000000000 1000000000 1000000000

#### Output
1999999998

#### Explanation
It is optimal to connect the first point of Leaf Left with the first of Leaf Right, and the last point of Leaf Left with the last of Leaf Right, satisfying the connectivity conditions efficiently given the values.

## Input Format
- The first line contains an integer n, the number of anchor points in each leaf.
- The second line contains n integers representing the surface textures of Leaf Left.
- The third line contains n integers representing the surface textures of Leaf Right.

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
