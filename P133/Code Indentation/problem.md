## Title
Code Indentation

## Slug
code-indentation

## Difficulty
Medium

## Description
Code blocks are indented. You want to draw a vertical guide that cuts through the fewest code blocks (passing through whitespace).

There is a file consisting of $n$ lines. Each line is composed of several blocks, each having a specific length (integers). The total length of every line is identical.

You need to draw a guide from the top to the bottom of the file that minimizes the number of blocks it cuts.

If the guide passes exactly through the whitespace between two blocks, it is **not** considered as cutting a block. However, you cannot place the guide at the very left or the very right of the file.

Given the 2D array `structure` containing the lengths of the blocks in each line, return the minimum number of blocks cut.

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
We can draw a guide at distance 4 from the left.
- Line 1: 1+2+2=5 (Cut)
- Line 2: 3+1=4 (Whitespace)
- Line 3: 1+3=4 (Whitespace)
- Line 4: 2 (Cut)
- Line 5: 3+1=4 (Whitespace)
- Line 6: 1+3=4 (Whitespace)
The guide cuts lines 1 and 4. Total: 2.

### 2

#### Input
3
1
1
1

#### Output
3

#### Explanation
There are no internal whitespaces. Any guide drawn must cut all 3 blocks.

## Input Format
- The first line contains an integer $n$, the number of lines.
- The next $n$ lines each contain space-separated integers representing the lengths of the blocks in that line.

## Output Format
- Return a single integer representing the minimum number of blocks cut.

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

