## Title
Solar Array

## Slug
solar-array

## Difficulty
Medium

## Description
Panels are arranged in rows. A shadow falls across the array, covering the fewest panels.

There is a array consisting of $n$ rows. Each row is composed of several panels, each having a specific width (integers). The total width of every row is identical.

You need to cast a shadow from the top to the bottom of the array that minimizes the number of panels it covers.

If the shadow passes exactly through the walkway between two panels, it is **not** considered as covering a panel. However, you cannot place the shadow at the very left or the very right of the array.

Given the 2D array `structure` containing the widths of the panels in each row, return the minimum number of panels covered.

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
We can cast a shadow at distance 4 from the left.
- Row 1: 1+2+2=5 (Cover)
- Row 2: 3+1=4 (Walkway)
- Row 3: 1+3=4 (Walkway)
- Row 4: 2 (Cover)
- Row 5: 3+1=4 (Walkway)
- Row 6: 1+3=4 (Walkway)
The shadow covers rows 1 and 4. Total: 2.

### 2

#### Input
3
1
1
1

#### Output
3

#### Explanation
There are no internal walkways. Any shadow drawn must cover all 3 panels.

## Input Format
- The first line contains an integer $n$, the number of rows.
- The next $n$ lines each contain space-separated integers representing the widths of the panels in that row.

## Output Format
- Return a single integer representing the minimum number of panels covered.

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

