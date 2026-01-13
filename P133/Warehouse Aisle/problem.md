## Title
Warehouse Aisle

## Slug
warehouse-aisle

## Difficulty
Medium

## Description
Pallets are stacked in rows. A forklift needs to drive straight through, moving the fewest pallets.

There is a warehouse consisting of $n$ rows. Each row is composed of several pallets, each having a specific width (integers). The total width of every row is identical.

You need to drive a path from the dock to the office of the warehouse that minimizes the number of pallets it hits.

If the path passes exactly through the space between two pallets, it is **not** considered as hitting a pallet. However, you cannot place the path at the very left or the very right of the warehouse.

Given the 2D array `structure` containing the widths of the pallets in each row, return the minimum number of pallets hit.

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
We can drive a path at distance 4 from the left.
- Row 1: 1+2+2=5 (Hit)
- Row 2: 3+1=4 (Space)
- Row 3: 1+3=4 (Space)
- Row 4: 2 (Hit)
- Row 5: 3+1=4 (Space)
- Row 6: 1+3=4 (Space)
The path hits rows 1 and 4. Total: 2.

### 2

#### Input
3
1
1
1

#### Output
3

#### Explanation
There are no internal spaces. Any path drawn must hit all 3 pallets.

## Input Format
- The first line contains an integer $n$, the number of rows.
- The next $n$ lines each contain space-separated integers representing the widths of the pallets in that row.

## Output Format
- Return a single integer representing the minimum number of pallets hit.

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

