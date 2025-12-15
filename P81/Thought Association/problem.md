## Title
Thought Association

## Slug
thought-association

## Difficulty
Medium

## Description
A mind jumps from Idea 1 to Idea n.

The brain has `n` ideas and `m` directed associations. Associations may repeat between the same pair of ideas and self-loops are allowed. A train of thought of length `k` is a sequence of exactly `k` directed associations; ideas and associations may be visited multiple times.

Given `n`, `m`, `k` and a list of the `m` directed associations (each association given as two integers `u` `v` meaning a directed association from `u` to `v`), compute the number of distinct trains of thought that start at idea 1 and end at idea `n` with length exactly `k`. Output the answer modulo 1000000007.

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
We have 3 ideas. We want the number of directed trains of thought of length 8 from idea 1 to idea 3.
Valid length-8 trains of thought:
1 -> 2 -> 3 -> 1 -> 2 -> 3 -> 1 -> 2 -> 3
1 -> 2 -> 3 -> 2 -> 3 -> 1 -> 2 -> 3
There are 2 such trains of thought.

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
Assuming the graph has associations 1->2 and 2->3, the only train of thought of length 2 from idea 1 to idea 3 is:
1 -> 2 -> 3

## Input Format
- The first line contains three integers n, m, and k: the number of ideas, associations, and the required train of thought length.
- The next m lines describe the associations. Each line contains two integers u and v, indicating a directed association from idea u to idea v.

## Output Format
- Return single integer: the number of trains of thought modulo 10^9+7.

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
