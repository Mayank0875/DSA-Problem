## Title
Barcode Scanner

## Slug
barcode-scanner

## Difficulty
Medium

## Description
Stacked barcodes are misaligned. A scanner laser tries to pass through white spaces to calibrate.

There is a stack consisting of $n$ codes. Each code is composed of several black bars, each having a specific width (integers). The total width of every code is identical.

You need to aim a laser from the top to the bottom of the stack that minimizes the number of black bars it hits.

If the laser passes exactly through the white space between two black bars, it is **not** considered as hitting a bar. However, you cannot place the laser at the very left or the very right of the stack.

Given the 2D array `structure` containing the widths of the black bars in each code, return the minimum number of black bars hit.

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
We can aim a laser at distance 4 from the left.
- Code 1: 1+2+2=5 (Hit)
- Code 2: 3+1=4 (Space)
- Code 3: 1+3=4 (Space)
- Code 4: 2 (Hit)
- Code 5: 3+1=4 (Space)
- Code 6: 1+3=4 (Space)
The laser hits codes 1 and 4. Total: 2.

### 2

#### Input
3
1
1
1

#### Output
3

#### Explanation
There are no internal white spaces. Any laser drawn must hit all 3 black bars.

## Input Format
- The first line contains an integer $n$, the number of codes.
- The next $n$ lines each contain space-separated integers representing the widths of the black bars in that code.

## Output Format
- Return a single integer representing the minimum number of black bars hit.

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

