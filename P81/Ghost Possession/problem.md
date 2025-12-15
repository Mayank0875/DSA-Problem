## Title
Ghost Possession

## Slug
ghost-possession

## Difficulty
Medium

## Description
A spirit jumps from Host 1 to Host n.

The haunted house has `n` hosts and `m` directed possessions. Possessions may repeat between the same pair of hosts and self-loops are allowed. A haunting of length `k` is a sequence of exactly `k` directed possessions; hosts and possessions may be visited multiple times.

Given `n`, `m`, `k` and a list of the `m` directed possessions (each possession given as two integers `u` `v` meaning a directed possession from `u` to `v`), compute the number of distinct hauntings that start at host 1 and end at host `n` with length exactly `k`. Output the answer modulo 1000000007.

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
We have 3 hosts. We want the number of directed hauntings of length 8 from host 1 to host 3.
Valid length-8 hauntings:
1 -> 2 -> 3 -> 1 -> 2 -> 3 -> 1 -> 2 -> 3
1 -> 2 -> 3 -> 2 -> 3 -> 1 -> 2 -> 3
There are 2 such hauntings.

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
Assuming the graph has possessions 1->2 and 2->3, the only haunting of length 2 from host 1 to host 3 is:
1 -> 2 -> 3

## Input Format
- The first line contains three integers n, m, and k: the number of hosts, possessions, and the required haunting length.
- The next m lines describe the possessions. Each line contains two integers u and v, indicating a directed possession from host u to host v.

## Output Format
- Return single integer: the number of hauntings modulo 10^9+7.

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
