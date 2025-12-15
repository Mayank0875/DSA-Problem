## Title
Computer Chip Data

## Slug
computer-chip-data

## Difficulty
Medium

## Description
Data bits travel from the CPU (node 1) to Memory (node n).

The microchip has `n` gates and `m` directed wires. Wires may repeat between the same pair of gates and self-loops are allowed. A signal path of length `k` is a sequence of exactly `k` directed wires; gates and wires may be visited multiple times.

Given `n`, `m`, `k` and a list of the `m` directed wires (each wire given as two integers `u` `v` meaning a directed wire from `u` to `v`), compute the number of distinct signal paths that start at gate 1 and end at gate `n` with length exactly `k`. Output the answer modulo 1000000007.

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
We have 3 gates. We want the number of directed signal paths of length 8 from gate 1 to gate 3.
Valid length-8 signal paths:
1 -> 2 -> 3 -> 1 -> 2 -> 3 -> 1 -> 2 -> 3
1 -> 2 -> 3 -> 2 -> 3 -> 1 -> 2 -> 3
There are 2 such signal paths.

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
Assuming the graph has wires 1->2 and 2->3, the only signal path of length 2 from gate 1 to gate 3 is:
1 -> 2 -> 3

## Input Format
- The first line contains three integers n, m, and k: the number of gates, wires, and the required signal path length.
- The next m lines describe the wires. Each line contains two integers u and v, indicating a directed wire from gate u to gate v.

## Output Format
- Return single integer: the number of signal paths modulo 10^9+7.

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
