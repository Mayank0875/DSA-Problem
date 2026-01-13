## Title
Tetris Stack

## Slug
tetris-stack

## Difficulty
Medium

## Description
Blocks are stacked. A laser shoots down, destroying the fewest blocks.

There is a grid consisting of $n$ rows. Each row is composed of several blocks, each having a specific width (integers). The total width of every row is identical.

You need to shoot a laser from the top to the bottom of the grid that minimizes the number of blocks it hits.

If the laser passes exactly through the empty cell between two blocks, it is **not** considered as hitting a block. However, you cannot place the laser at the very left or the very right of the grid.

Given the 2D array `structure` containing the widths of the blocks in each row, return the minimum number of blocks hit.

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
We can shoot a laser at distance 4 from the left.
- Row 1: 1+2+2=5 (Hit)
- Row 2: 3+1=4 (Empty)
- Row 3: 1+3=4 (Empty)
- Row 4: 2 (Hit)
- Row 5: 3+1=4 (Empty)
- Row 6: 1+3=4 (Empty)
The laser hits rows 1 and 4. Total: 2.

### 2

#### Input
3
1
1
1

#### Output
3

#### Explanation
There are no internal empty cells. Any laser drawn must hit all 3 blocks.

## Input Format
- The first line contains an integer $n$, the number of rows.
- The next $n$ lines each contain space-separated integers representing the widths of the blocks in that row.

## Output Format
- Return a single integer representing the minimum number of blocks hit.

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

