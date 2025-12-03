## Title
Beehive Frame Support

## Slug
beehive-frame-support

## Difficulty
Medium

## Description
Two honeycomb frames need wax bridges to stay connected if the comb breaks.

Two parallel frames, Frame Front and Frame Back, each contain n cells arranged in a line.
Frame Front has an array `a` representing the honey volume of each cell.
Frame Back has an array `b` representing the honey volume of each cell.

Inside each frame, adjacent cells are already connected by internal wax walls.

You must establish inter-frame bridges connecting some cells of Frame Front to some cells of Frame Back.

The cost to create a bridge between cell i of Frame Front and cell j of Frame Back is:
absolute value of (a[i] - b[j]).

**Fault-tolerance requirement:**
The final network must remain fully connected even if any single cell is removed (from either Frame Front or Frame Back).
If one cell fails and disappears along with all its connections, the remaining cells must still form a single connected network.

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
It's optimal to connect four pairs of cells:
1. cell 1 from Frame Front with cell 2 from Frame Back: cost |1-4| = 3.
2. cell 3 from Frame Front with cell 2 from Frame Back: cost |1-4| = 3.
3. cell 2 from Frame Front with cell 1 from Frame Back: cost |10-20| = 10.
4. cell 2 from Frame Front with cell 3 from Frame Back: cost |10-25| = 15.
Total cost: 3 + 3 + 10 + 15 = 31.

### 2

#### Input
4
1 1 1 1
1000000000 1000000000 1000000000 1000000000

#### Output
1999999998

#### Explanation
It is optimal to connect the first cell of Frame Front with the first of Frame Back, and the last cell of Frame Front with the last of Frame Back, satisfying the connectivity conditions efficiently given the values.

## Input Format
- The first line contains an integer n, the number of cells in each frame.
- The second line contains n integers representing the honey volumes of Frame Front.
- The third line contains n integers representing the honey volumes of Frame Back.

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
