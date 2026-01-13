## Title
Ceramic Tile Cutting

## Slug
ceramic-tile-cutting

## Difficulty
Medium

## Description
A mosaic is made of rows of tiles. You need to cut the entire sheet, breaking as few tiles as possible.

There is a mosaic sheet consisting of $n$ rows. Each row is composed of several tiles, each having a specific width (integers). The total width of every row is identical.

You need to make a cut from the top to the bottom of the mosaic sheet that minimizes the number of tiles it breaks.

If the cut passes exactly through the grout line between two tiles, it is **not** considered as breaking a tile. However, you cannot place the cut at the very left edge or the very right edge of the mosaic sheet.

Given the 2D array `structure` containing the widths of the tiles in each row, return the minimum number of tiles broken.

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
We can make a cut at distance 4 from the left edge.
- Row 1: 1+2+2=5 (Break)
- Row 2: 3+1=4 (Grout)
- Row 3: 1+3=4 (Grout)
- Row 4: 2 (Break)
- Row 5: 3+1=4 (Grout)
- Row 6: 1+3=4 (Grout)
The cut breaks rows 1 and 4. Total: 2.

### 2

#### Input
3
1
1
1

#### Output
3

#### Explanation
There are no internal grout lines. Any cut drawn must break all 3 tiles.

## Input Format
- The first line contains an integer $n$, the number of rows.
- The next $n$ lines each contain space-separated integers representing the widths of the tiles in that row.

## Output Format
- Return a single integer representing the minimum number of tiles broken.

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

