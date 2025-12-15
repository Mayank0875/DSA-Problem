## Title
Social Rumor Mill

## Slug
social-rumor-mill

## Difficulty
Medium

## Description
A rumor spreads from Person 1 to Person n.

The social circle has `n` people and `m` directed conversations. Conversations may repeat between the same pair of people and self-loops are allowed. A gossip chain of length `k` is a sequence of exactly `k` directed conversations; people and conversations may be visited multiple times.

Given `n`, `m`, `k` and a list of the `m` directed conversations (each conversation given as two integers `u` `v` meaning a directed conversation from `u` to `v`), compute the number of distinct gossip chains that start at person 1 and end at person `n` with length exactly `k`. Output the answer modulo 1000000007.

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
We have 3 people. We want the number of directed gossip chains of length 8 from person 1 to person 3.
Valid length-8 gossip chains:
1 -> 2 -> 3 -> 1 -> 2 -> 3 -> 1 -> 2 -> 3
1 -> 2 -> 3 -> 2 -> 3 -> 1 -> 2 -> 3
There are 2 such gossip chains.

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
Assuming the graph has conversations 1->2 and 2->3, the only gossip chain of length 2 from person 1 to person 3 is:
1 -> 2 -> 3

## Input Format
- The first line contains three integers n, m, and k: the number of people, conversations, and the required gossip chain length.
- The next m lines describe the conversations. Each line contains two integers u and v, indicating a directed conversation from person u to person v.

## Output Format
- Return single integer: the number of gossip chains modulo 10^9+7.

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
