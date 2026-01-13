## Title
Cake Slicing

## Slug
cake-slicing

## Difficulty
Medium

## Description
A layered cake has fruit chunks embedded in each layer. You want to slice the cake while cutting through the fewest fruit chunks.

There is a cake consisting of $n$ layers. Each layer is composed of several fruit chunks, each having a specific width (integers). The total width of every layer is identical.

You need to cut a slice from the top to the bottom of the cake that minimizes the number of fruit chunks it slices through.

If the slice passes exactly through the icing gap between two fruit chunks, it is **not** considered as slicing a fruit chunk. However, you cannot place the slice at the very left edge or the very right edge of the cake.

Given the 2D array `structure` containing the widths of the fruit chunks in each layer, return the minimum number of fruit chunks sliced.

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
We can cut a slice at distance 4 from the left edge.
- Layer 1: 1+2+2=5 (Slice)
- Layer 2: 3+1=4 (Gap)
- Layer 3: 1+3=4 (Gap)
- Layer 4: 2 (Slice)
- Layer 5: 3+1=4 (Gap)
- Layer 6: 1+3=4 (Gap)
The slice slices through layers 1 and 4. Total: 2.

### 2

#### Input
3
1
1
1

#### Output
3

#### Explanation
There are no internal icing gaps. Any slice drawn must slice through all 3 fruit chunks.

## Input Format
- The first line contains an integer $n$, the number of layers.
- The next $n$ lines each contain space-separated integers representing the widths of the fruit chunks in that layer.

## Output Format
- Return a single integer representing the minimum number of fruit chunks sliced.

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

