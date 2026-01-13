## Title
Laser Security Grid

## Slug
laser-security-grid

## Difficulty
Medium

## Description
Laser beams block a corridor at intervals. An intruder wants to run straight, breaking the fewest beams.

There is a corridor consisting of $n$ scanners. Each scanner line is composed of several beams, each having a specific width (integers). The total width of every scanner line is identical.

You need to run a path from the entry to the exit of the corridor that minimizes the number of beams it breaks.

If the path passes exactly through the safe zone between two beams, it is **not** considered as breaking a beam. However, you cannot place the path at the very left wall or the very right wall of the corridor.

Given the 2D array `structure` containing the widths of the beams in each scanner line, return the minimum number of beams broken.

## Examples

### 1

#### Input
6
1 2 2 1
3 1 2
1 3 2
2 4
3 1 2
1 3 1 1

#### Output
2

#### Explanation
The total width is 6.
We can run a path at distance 4 from the left wall.
- Line 1: 1+2+2=5 (Break)
- Line 2: 3+1=4 (Safe zone)
- Line 3: 1+3=4 (Safe zone)
- Line 4: 2 (Break)
- Line 5: 3+1=4 (Safe zone)
- Line 6: 1+3=4 (Safe zone)
The path breaks scanners 1 and 4. Total: 2.

### 2

#### Input
3
1
1
1

#### Output
3

#### Explanation
There are no internal safe zones. Any path drawn must break all 3 beams.

## Input Format
- The first line contains an integer $n$, the number of scanners.
- The next $n$ lines each contain space-separated integers representing the widths of the beams in that scanner line.

## Output Format
- Return a single integer representing the minimum number of beams broken.

## Constraints
- 1 ≤ n ≤ 10^4
- 1 <= structure[i].length <= 10^4
- The sum of elements in each row is the same.
- 1 <= structure[i][j] <= 2^31 - 1

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, prefix-sum

