## Title
Network Cables

## Slug
network-cables

## Difficulty
Medium

## Description
Bundles of cables run in parallel. A mouse chews through the bundle, severing the fewest cables.

There is a bundle consisting of $n$ layers. Each layer is composed of several cables, each having a specific thickness (integers). The total thickness of every layer is identical.

You need to chew a path from the top to the bottom of the bundle that minimizes the number of cables it severs.

If the path passes exactly through the air gap between two cables, it is **not** considered as severing a cable. However, you cannot place the path at the very left or the very right of the bundle.

Given the 2D array `structure` containing the thicknesss of the cables in each layer, return the minimum number of cables severed.

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
The total thickness is 6.
We can chew a path at distance 4 from the left.
- Layer 1: 1+2+2=5 (Sever)
- Layer 2: 3+1=4 (Gap)
- Layer 3: 1+3=4 (Gap)
- Layer 4: 2 (Sever)
- Layer 5: 3+1=4 (Gap)
- Layer 6: 1+3=4 (Gap)
The path severs layers 1 and 4. Total: 2.

### 2

#### Input
3
1
1
1

#### Output
3

#### Explanation
There are no internal air gaps. Any path drawn must sever all 3 cables.

## Input Format
- The first line contains an integer $n$, the number of layers.
- The next $n$ lines each contain space-separated integers representing the thicknesss of the cables in that layer.

## Output Format
- Return a single integer representing the minimum number of cables severed.

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

