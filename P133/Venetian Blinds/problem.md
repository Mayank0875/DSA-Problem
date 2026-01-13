## Title
Venetian Blinds

## Slug
venetian-blinds

## Difficulty
Medium

## Description
Blinds have slats. A string runs down, touching the fewest slats (going through holes).

There is a window consisting of $n$ levels. Each level is composed of several slats, each having a specific width (integers). The total width of every level is identical.

You need to run a string from the top to the bottom of the window that minimizes the number of slats it touches.

If the string passes exactly through the hole between two slats, it is **not** considered as touching a slat. However, you cannot place the string at the very left or the very right of the window.

Given the 2D array `structure` containing the widths of the slats in each level, return the minimum number of slats touched.

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
We can run a string at distance 4 from the left.
- Level 1: 1+2+2=5 (Touch)
- Level 2: 3+1=4 (Hole)
- Level 3: 1+3=4 (Hole)
- Level 4: 2 (Touch)
- Level 5: 3+1=4 (Hole)
- Level 6: 1+3=4 (Hole)
The string touches levels 1 and 4. Total: 2.

### 2

#### Input
3
1
1
1

#### Output
3

#### Explanation
There are no internal holes. Any string drawn must touch all 3 slats.

## Input Format
- The first line contains an integer $n$, the number of levels.
- The next $n$ lines each contain space-separated integers representing the widths of the slats in that level.

## Output Format
- Return a single integer representing the minimum number of slats touched.

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

