## Title
Garden Hedges

## Slug
garden-hedges

## Difficulty
Medium

## Description
Hedges are planted in rows. You need to cut a path through the fewest hedges.

There is a garden consisting of $n$ rows. Each row is composed of several hedges, each having a specific length (integers). The total length of every row is identical.

You need to cut a path from the front to the back of the garden that minimizes the number of hedges it cuts.

If the path passes exactly through the opening between two hedges, it is **not** considered as cutting a hedge. However, you cannot place the path at the very left or the very right of the garden.

Given the 2D array `structure` containing the lengths of the hedges in each row, return the minimum number of hedges cut.

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
The total length is 6.
We can cut a path at distance 4 from the left.
- Row 1: 1+2+2=5 (Cut)
- Row 2: 3+1=4 (Opening)
- Row 3: 1+3=4 (Opening)
- Row 4: 2 (Cut)
- Row 5: 3+1=4 (Opening)
- Row 6: 1+3=4 (Opening)
The path cuts rows 1 and 4. Total: 2.

### 2

#### Input
3
1
1
1

#### Output
3

#### Explanation
There are no internal openings. Any path drawn must cut all 3 hedges.

## Input Format
- The first line contains an integer $n$, the number of rows.
- The next $n$ lines each contain space-separated integers representing the lengths of the hedges in that row.

## Output Format
- Return a single integer representing the minimum number of hedges cut.

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

