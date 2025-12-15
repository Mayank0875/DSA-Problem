## Title
Spy Network Message

## Slug
spy-network-message

## Difficulty
Medium

## Description
An encoded message is passed from Agent 1 to the Handler (node n).

The spy ring has `n` agents and `m` directed handoffs. Handoffs may repeat between the same pair of agents and self-loops are allowed. A transmission chain of length `k` is a sequence of exactly `k` directed handoffs; agents and handoffs may be visited multiple times.

Given `n`, `m`, `k` and a list of the `m` directed handoffs (each handoff given as two integers `u` `v` meaning a directed handoff from `u` to `v`), compute the number of distinct transmission chains that start at agent 1 and end at agent `n` with length exactly `k`. Output the answer modulo 1000000007.

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
We have 3 agents. We want the number of directed transmission chains of length 8 from agent 1 to agent 3.
Valid length-8 transmission chains:
1 -> 2 -> 3 -> 1 -> 2 -> 3 -> 1 -> 2 -> 3
1 -> 2 -> 3 -> 2 -> 3 -> 1 -> 2 -> 3
There are 2 such transmission chains.

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
Assuming the graph has handoffs 1->2 and 2->3, the only transmission chain of length 2 from agent 1 to agent 3 is:
1 -> 2 -> 3

## Input Format
- The first line contains three integers n, m, and k: the number of agents, handoffs, and the required transmission chain length.
- The next m lines describe the handoffs. Each line contains two integers u and v, indicating a directed handoff from agent u to agent v.

## Output Format
- Return single integer: the number of transmission chains modulo 10^9+7.

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
