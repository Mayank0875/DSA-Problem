## Title
Tent Guy Lines

## Slug
tent-guy-lines

## Difficulty
Medium

## Description
Two rows of tent poles need cross-ropes to stay stable in high winds.

Two parallel rows, Left Poles and Right Poles, each contain n poles arranged in a line.
Left Poles has an array `a` representing the height of each pole.
Right Poles has an array `b` representing the height of each pole.

Inside each row, adjacent poles are already connected by internal canvas tension.

You must establish inter-row guy lines connecting some poles of Left Poles to some poles of Right Poles.

The cost to create a line between pole i of Left Poles and pole j of Right Poles is:
absolute value of (a[i] - b[j]).

**Fault-tolerance requirement:**
The final network must remain fully connected even if any single pole is removed (from either Left Poles or Right Poles).
If one pole fails and disappears along with all its connections, the remaining poles must still form a single connected network.

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
It's optimal to connect four pairs of poles:
1. pole 1 from Left Poles with pole 2 from Right Poles: cost |1-4| = 3.
2. pole 3 from Left Poles with pole 2 from Right Poles: cost |1-4| = 3.
3. pole 2 from Left Poles with pole 1 from Right Poles: cost |10-20| = 10.
4. pole 2 from Left Poles with pole 3 from Right Poles: cost |10-25| = 15.
Total cost: 3 + 3 + 10 + 15 = 31.

### 2

#### Input
4
1 1 1 1
1000000000 1000000000 1000000000 1000000000

#### Output
1999999998

#### Explanation
It is optimal to connect the first pole of Left Poles with the first of Right Poles, and the last pole of Left Poles with the last of Right Poles, satisfying the connectivity conditions efficiently given the values.

## Input Format
- The first line contains an integer n, the number of poles in each row.
- The second line contains n integers representing the heights of Left Poles.
- The third line contains n integers representing the heights of Right Poles.

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
