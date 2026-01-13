## Title
Subway Tiles

## Slug
subway-tiles

## Difficulty
Medium

## Description
Tiles line a tunnel. A crack runs down, cracking the fewest tiles.

There is a wall consisting of $n$ rows. Each row is composed of several tiles, each having a specific width (integers). The total width of every row is identical.

You need to form a crack from the ceiling to the floor of the wall that minimizes the number of tiles it cracks.

If the crack passes exactly through the grout between two tiles, it is **not** considered as cracking a tile. However, you cannot place the crack at the very left or the very right of the wall.

Given the 2D array `structure` containing the widths of the tiles in each row, return the minimum number of tiles cracked.

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
We can form a crack at distance 4 from the left.
- Row 1: 1+2+2=5 (Crack)
- Row 2: 3+1=4 (Grout)
- Row 3: 1+3=4 (Grout)
- Row 4: 2 (Crack)
- Row 5: 3+1=4 (Grout)
- Row 6: 1+3=4 (Grout)
The crack cracks rows 1 and 4. Total: 2.

### 2

#### Input
3
1
1
1

#### Output
3

#### Explanation
There are no internal grouts. Any crack drawn must crack all 3 tiles.

## Input Format
- The first line contains an integer $n$, the number of rows.
- The next $n$ lines each contain space-separated integers representing the widths of the tiles in that row.

## Output Format
- Return a single integer representing the minimum number of tiles cracked.

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

