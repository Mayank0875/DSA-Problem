## Title
Cemetery Plots

## Slug
cemetery-plots

## Difficulty
Medium

## Description
Graves are in rows. A ghost floats through, passing through the fewest headstones.

There is a graveyard consisting of $n$ rows. Each row is composed of several headstones, each having a specific width (integers). The total width of every row is identical.

You need to float a path from the gate to the wall of the graveyard that minimizes the number of headstones it phases through.

If the path passes exactly through the grass between two headstones, it is **not** considered as phasing through a headstone. However, you cannot place the path at the very left or the very right of the graveyard.

Given the 2D array `structure` containing the widths of the headstones in each row, return the minimum number of headstones phased through.

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
We can float a path at distance 4 from the left.
- Row 1: 1+2+2=5 (Phase)
- Row 2: 3+1=4 (Grass)
- Row 3: 1+3=4 (Grass)
- Row 4: 2 (Phase)
- Row 5: 3+1=4 (Grass)
- Row 6: 1+3=4 (Grass)
The path phases through rows 1 and 4. Total: 2.

### 2

#### Input
3
1
1
1

#### Output
3

#### Explanation
There are no internal grasss. Any path drawn must phase through all 3 headstones.

## Input Format
- The first line contains an integer $n$, the number of rows.
- The next $n$ lines each contain space-separated integers representing the widths of the headstones in that row.

## Output Format
- Return a single integer representing the minimum number of headstones phased through.

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

