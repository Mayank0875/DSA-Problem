## Title
Timber Mill Cutting

## Slug
timber-mill-cutting

## Difficulty
Medium

## Description
A lumber mill processes logs stacked in layers. Each layer has sections of good wood separated by knots.

There is a stack of logs consisting of $n$ layers. Each layer is composed of several sections, each having a specific length (integers). The total length of every layer is identical.

You need to make a vertical cut from the top to the bottom of the stack of logs that minimizes the number of sections it cuts through.

If the vertical cut passes exactly through the knot between two sections, it is **not** considered as cutting a section. However, you cannot place the vertical cut at the very left edge or the very right edge of the stack of logs.

Given the 2D array `structure` containing the lengths of the sections in each layer, return the minimum number of sections cut.

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
We can make a vertical cut at distance 4 from the left edge.
- Layer 1: 1+2+2=5 (Cut)
- Layer 2: 3+1=4 (Knot)
- Layer 3: 1+3=4 (Knot)
- Layer 4: 2 (Cut)
- Layer 5: 3+1=4 (Knot)
- Layer 6: 1+3=4 (Knot)
The vertical cut cuts through layers 1 and 4. Total: 2.

### 2

#### Input
3
1
1
1

#### Output
3

#### Explanation
There are no internal knots. Any vertical cut drawn must cut through all 3 sections.

## Input Format
- The first line contains an integer $n$, the number of layers.
- The next $n$ lines each contain space-separated integers representing the lengths of the sections in that layer.

## Output Format
- Return a single integer representing the minimum number of sections cut.

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

