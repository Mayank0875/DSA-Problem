## Title
Barcode Printer

## Slug
barcode-printer

## Difficulty
Medium

## Description
A printer head is misaligned. It prints a line down the sheet, ruining the fewest barcodes.

There is a sheet consisting of $n$ rows. Each row is composed of several barcodes, each having a specific width (integers). The total width of every row is identical.

You need to print a line from the top to the bottom of the sheet that minimizes the number of barcodes it ruins.

If the line passes exactly through the margin between two barcodes, it is **not** considered as ruining a barcode. However, you cannot place the line at the very left or the very right of the sheet.

Given the 2D array `structure` containing the widths of the barcodes in each row, return the minimum number of barcodes ruined.

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
We can print a line at distance 4 from the left.
- Row 1: 1+2+2=5 (Ruin)
- Row 2: 3+1=4 (Margin)
- Row 3: 1+3=4 (Margin)
- Row 4: 2 (Ruin)
- Row 5: 3+1=4 (Margin)
- Row 6: 1+3=4 (Margin)
The line ruins rows 1 and 4. Total: 2.

### 2

#### Input
3
1
1
1

#### Output
3

#### Explanation
There are no internal margins. Any line drawn must ruin all 3 barcodes.

## Input Format
- The first line contains an integer $n$, the number of rows.
- The next $n$ lines each contain space-separated integers representing the widths of the barcodes in that row.

## Output Format
- Return a single integer representing the minimum number of barcodes ruined.

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

