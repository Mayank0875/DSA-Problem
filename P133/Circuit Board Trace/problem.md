## Title
Circuit Board Trace

## Slug
circuit-board-trace

## Difficulty
Medium

## Description
A PCB has component blocks. You need to route a trace vertically crossing the fewest components.

There is a board consisting of $n$ layers. Each layer is composed of several components, each having a specific width (integers). The total width of every layer is identical.

You need to route a trace from the top to the bottom of the board that minimizes the number of components it crosses.

If the trace passes exactly through the gap between two components, it is **not** considered as crossing a component. However, you cannot place the trace at the very left edge or the very right edge of the board.

Given the 2D array `structure` containing the widths of the components in each layer, return the minimum number of components crossed.

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
We can route a trace at distance 4 from the left edge.
- Layer 1: 1+2+2=5 (Cross)
- Layer 2: 3+1=4 (Gap)
- Layer 3: 1+3=4 (Gap)
- Layer 4: 2 (Cross)
- Layer 5: 3+1=4 (Gap)
- Layer 6: 1+3=4 (Gap)
The trace crosses layers 1 and 4. Total: 2.

### 2

#### Input
3
1
1
1

#### Output
3

#### Explanation
There are no internal gaps. Any trace drawn must cross all 3 components.

## Input Format
- The first line contains an integer $n$, the number of layers.
- The next $n$ lines each contain space-separated integers representing the widths of the components in that layer.

## Output Format
- Return a single integer representing the minimum number of components crossed.

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

