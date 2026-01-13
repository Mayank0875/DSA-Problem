## Title
Glacier Crevasses

## Slug
glacier-crevasses

## Difficulty
Medium

## Description
An ice sheet has crevasses. An explorer wants to walk straight, jumping over the fewest crevasses.

There is a glacier consisting of $n$ sections. Each section is composed of several crevasses, each having a specific width (integers). The total width of every section is identical.

You need to walk a path from the camp to the summit of the glacier that minimizes the number of crevasses it jumps.

If the path passes exactly through the ice between two crevasses, it is **not** considered as jumping a crevasse. However, you cannot place the path at the very left or the very right of the glacier.

Given the 2D array `structure` containing the widths of the crevasses in each section, return the minimum number of crevasses jumped.

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
We can walk a path at distance 4 from the left.
- Section 1: 1+2+2=5 (Jump)
- Section 2: 3+1=4 (Ice)
- Section 3: 1+3=4 (Ice)
- Section 4: 2 (Jump)
- Section 5: 3+1=4 (Ice)
- Section 6: 1+3=4 (Ice)
The path jumps sections 1 and 4. Total: 2.

### 2

#### Input
3
1
1
1

#### Output
3

#### Explanation
There are no internal ices. Any path drawn must jump all 3 crevasses.

## Input Format
- The first line contains an integer $n$, the number of sections.
- The next $n$ lines each contain space-separated integers representing the widths of the crevasses in that section.

## Output Format
- Return a single integer representing the minimum number of crevasses jumped.

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

