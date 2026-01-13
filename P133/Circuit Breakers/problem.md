## Title
Circuit Breakers

## Slug
circuit-breakers

## Difficulty
Medium

## Description
Breakers are aligned in a panel. A fault line arcs down, tripping the fewest breakers.

There is a panel consisting of $n$ rows. Each row is composed of several breakers, each having a specific width (integers). The total width of every row is identical.

You need to arc a fault from the top to the bottom of the panel that minimizes the number of breakers it trips.

If the fault passes exactly through the spacer between two breakers, it is **not** considered as tripping a breaker. However, you cannot place the fault at the very left or the very right of the panel.

Given the 2D array `structure` containing the widths of the breakers in each row, return the minimum number of breakers tripped.

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
We can arc a fault at distance 4 from the left.
- Row 1: 1+2+2=5 (Trip)
- Row 2: 3+1=4 (Spacer)
- Row 3: 1+3=4 (Spacer)
- Row 4: 2 (Trip)
- Row 5: 3+1=4 (Spacer)
- Row 6: 1+3=4 (Spacer)
The fault trips rows 1 and 4. Total: 2.

### 2

#### Input
3
1
1
1

#### Output
3

#### Explanation
There are no internal spacers. Any fault drawn must trip all 3 breakers.

## Input Format
- The first line contains an integer $n$, the number of rows.
- The next $n$ lines each contain space-separated integers representing the widths of the breakers in that row.

## Output Format
- Return a single integer representing the minimum number of breakers tripped.

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

