## Title
Ecological Energy

## Slug
ecological-energy

## Difficulty
Medium

## Description
Energy transfers from Organism 1 to Organism n.

The food web has `n` organisms and `m` directed feeding events. Feeding events may repeat between the same pair of organisms and self-loops are allowed. A food chain of length `k` is a sequence of exactly `k` directed feeding events; organisms and feeding events may be visited multiple times.

Given `n`, `m`, `k` and a list of the `m` directed feeding events (each feeding event given as two integers `u` `v` meaning a directed feeding event from `u` to `v`), compute the number of distinct food chains that start at organism 1 and end at organism `n` with length exactly `k`. Output the answer modulo 1000000007.

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
We have 3 organisms. We want the number of directed food chains of length 8 from organism 1 to organism 3.
Valid length-8 food chains:
1 -> 2 -> 3 -> 1 -> 2 -> 3 -> 1 -> 2 -> 3
1 -> 2 -> 3 -> 2 -> 3 -> 1 -> 2 -> 3
There are 2 such food chains.

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
Assuming the graph has feeding events 1->2 and 2->3, the only food chain of length 2 from organism 1 to organism 3 is:
1 -> 2 -> 3

## Input Format
- The first line contains three integers n, m, and k: the number of organisms, feeding events, and the required food chain length.
- The next m lines describe the feeding events. Each line contains two integers u and v, indicating a directed feeding event from organism u to organism v.

## Output Format
- Return single integer: the number of food chains modulo 10^9+7.

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
