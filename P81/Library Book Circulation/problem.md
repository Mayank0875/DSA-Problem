## Title
Library Book Circulation

## Slug
library-book-circulation

## Difficulty
Medium

## Description
A book is transferred from Branch 1 to Branch n.

The library network has `n` branches and `m` directed transfers. Transfers may repeat between the same pair of branches and self-loops are allowed. A history of length `k` is a sequence of exactly `k` directed transfers; branches and transfers may be visited multiple times.

Given `n`, `m`, `k` and a list of the `m` directed transfers (each transfer given as two integers `u` `v` meaning a directed transfer from `u` to `v`), compute the number of distinct histories that start at branch 1 and end at branch `n` with length exactly `k`. Output the answer modulo 1000000007.

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
We have 3 branches. We want the number of directed histories of length 8 from branch 1 to branch 3.
Valid length-8 histories:
1 -> 2 -> 3 -> 1 -> 2 -> 3 -> 1 -> 2 -> 3
1 -> 2 -> 3 -> 2 -> 3 -> 1 -> 2 -> 3
There are 2 such histories.

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
Assuming the graph has transfers 1->2 and 2->3, the only history of length 2 from branch 1 to branch 3 is:
1 -> 2 -> 3

## Input Format
- The first line contains three integers n, m, and k: the number of branches, transfers, and the required history length.
- The next m lines describe the transfers. Each line contains two integers u and v, indicating a directed transfer from branch u to branch v.

## Output Format
- Return single integer: the number of histories modulo 10^9+7.

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
