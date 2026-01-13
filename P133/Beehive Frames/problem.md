## Title
Beehive Frames

## Slug
beehive-frames

## Difficulty
Medium

## Description
Honeycomb frames have brood cells. A varroa mite cutter cuts a line destroying the fewest cells.

There is a hive consisting of $n$ frames. Each frame is composed of several cells, each having a specific width (integers). The total width of every frame is identical.

You need to cut a line from the top to the bottom of the hive that minimizes the number of cells it destroys.

If the line passes exactly through the wax wall between two cells, it is **not** considered as destroying a cell. However, you cannot place the line at the very left or the very right of the hive.

Given the 2D array `structure` containing the widths of the cells in each frame, return the minimum number of cells destroyed.

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
We can cut a line at distance 4 from the left.
- Frame 1: 1+2+2=5 (Destroy)
- Frame 2: 3+1=4 (Wall)
- Frame 3: 1+3=4 (Wall)
- Frame 4: 2 (Destroy)
- Frame 5: 3+1=4 (Wall)
- Frame 6: 1+3=4 (Wall)
The line destroys frames 1 and 4. Total: 2.

### 2

#### Input
3
1
1
1

#### Output
3

#### Explanation
There are no internal wax walls. Any line drawn must destroy all 3 cells.

## Input Format
- The first line contains an integer $n$, the number of frames.
- The next $n$ lines each contain space-separated integers representing the widths of the cells in that frame.

## Output Format
- Return a single integer representing the minimum number of cells destroyed.

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

