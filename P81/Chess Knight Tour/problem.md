## Title
Chess Knight Tour

## Slug
chess-knight-tour

## Difficulty
Medium

## Description
A knight moves from Square 1 to Square n on a custom board.

The chessboard has `n` squares and `m` directed knight moves. Knight moves may repeat between the same pair of squares and self-loops are allowed. A tour of length `k` is a sequence of exactly `k` directed knight moves; squares and knight moves may be visited multiple times.

Given `n`, `m`, `k` and a list of the `m` directed knight moves (each knight move given as two integers `u` `v` meaning a directed knight move from `u` to `v`), compute the number of distinct tours that start at square 1 and end at square `n` with length exactly `k`. Output the answer modulo 1000000007.

## Examples

### 1

#### Input
3 4 8
1 2
2 3
3 1
3 2

#### Output
2

#### Explanation
We have 3 squares. We want the number of directed tours of length 8 from square 1 to square 3.
Valid length-8 tours:
1 -> 2 -> 3 -> 1 -> 2 -> 3 -> 1 -> 2 -> 3
1 -> 2 -> 3 -> 2 -> 3 -> 1 -> 2 -> 3
There are 2 such tours.

### 2

#### Input
3 4 2
1 2
2 3
3 1
3 2

#### Output
1

#### Explanation
Assuming the graph has knight moves 1->2 and 2->3, the only tour of length 2 from square 1 to square 3 is:
1 -> 2 -> 3

## Input Format
- The first line contains three integers n, m, and k: the number of squares, knight moves, and the required tour length.
- The next m lines describe the knight moves. Each line contains two integers u and v, indicating a directed knight move from square u to square v.

## Output Format
- Return single integer: the number of tours modulo 10^9+7.

## Constraints
- 1 ≤ n ≤ 100
- 1 ≤ m ≤ 10^5
- 1 ≤ k ≤ 10^18
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, dynamic-programming
