## Title
Rope Bridge Planks

## Slug
rope-bridge-planks

## Difficulty
Medium

## Description
A bridge has planks. You want to drop a stone that hits the fewest planks.

There is a bridge consisting of $n$ sections. Each section is composed of several planks, each having a specific width (integers). The total width of every section is identical.

You need to drop a stone from the top to the water of the bridge that minimizes the number of planks it hits.

If the stone passes exactly through the gap between two planks, it is **not** considered as hitting a plank. However, you cannot place the stone at the very left or the very right of the bridge.

Given the 2D array `structure` containing the widths of the planks in each section, return the minimum number of planks hit.

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
We can drop a stone at distance 4 from the left.
- Section 1: 1+2+2=5 (Hit)
- Section 2: 3+1=4 (Gap)
- Section 3: 1+3=4 (Gap)
- Section 4: 2 (Hit)
- Section 5: 3+1=4 (Gap)
- Section 6: 1+3=4 (Gap)
The stone hits sections 1 and 4. Total: 2.

### 2

#### Input
3
1
1
1

#### Output
3

#### Explanation
There are no internal gaps. Any stone drawn must hit all 3 planks.

## Input Format
- The first line contains an integer $n$, the number of sections.
- The next $n$ lines each contain space-separated integers representing the widths of the planks in that section.

## Output Format
- Return a single integer representing the minimum number of planks hit.

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

