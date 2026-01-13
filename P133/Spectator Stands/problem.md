## Title
Spectator Stands

## Slug
spectator-stands

## Difficulty
Medium

## Description
People are sitting in rows. A vendor wants to walk up the stairs passing the fewest seated groups.

There is a stadium consisting of $n$ rows. Each row is composed of several groups, each having a specific width (integers). The total width of every row is identical.

You need to walk a path from the bottom to the top of the stadium that minimizes the number of groups it disturbs.

If the path passes exactly through the aisle between two groups, it is **not** considered as disturbing a group. However, you cannot place the path at the very left or the very right of the stadium.

Given the 2D array `structure` containing the widths of the groups in each row, return the minimum number of groups disturbed.

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
We can walk a path at distance 4 from the left.
- Row 1: 1+2+2=5 (Disturb)
- Row 2: 3+1=4 (Aisle)
- Row 3: 1+3=4 (Aisle)
- Row 4: 2 (Disturb)
- Row 5: 3+1=4 (Aisle)
- Row 6: 1+3=4 (Aisle)
The path disturbs rows 1 and 4. Total: 2.

### 2

#### Input
3
1
1
1

#### Output
3

#### Explanation
There are no internal aisles. Any path drawn must disturb all 3 groups.

## Input Format
- The first line contains an integer $n$, the number of rows.
- The next $n$ lines each contain space-separated integers representing the widths of the groups in that row.

## Output Format
- Return a single integer representing the minimum number of groups disturbed.

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

