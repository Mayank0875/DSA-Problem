## Title
Network Traffic

## Slug
network-traffic

## Difficulty
Medium

## Description
A router buffers packets into queues.

The router has prepared $n$ packets arranged in a sequence. The $i$-th packet has a value of $a_i$.

These packets need to be grouped into queues. Every queue must hold the exact same number of packets, denoted by $k$. The grouping happens sequentially:
- The first $k$ packets go into the first queue.
- The second $k$ packets go into the second queue.
- ...
- The last $k$ packets go into the $(n/k)$-th queue.

Since every queue must have exactly $k$ packets, this grouping is only possible if $n$ is divisible by $k$ ($1 \le k \le n$).

The router wants to choose a valid $k$ such that the **difference between the maximum total value and the minimum total value** of the queues is maximized. If there is only one queue (i.e., $k=n$), the difference is 0.

Your task is to calculate this maximum possible difference over all valid choices of $k$.

## Examples

### 1

#### Input
2
1 2

#### Output
1

#### Explanation
Possible values for $k$ are divisors of 2: 1, 2.
- $k=1$: queue 1 has sum 1, queue 2 has sum 2. Difference = $|2-1| = 1$.
- $k=2$: Only one queue with sum $1+2=3$. Difference = 0.
Max difference is 1.

### 2

#### Input
4
10 10 10 10

#### Output
0

#### Explanation
All packets are equal. Regardless of $k$, all queues will have the same sum. Difference is always 0.

## Input Format
- The first line contains one integer $n$ — the number of packets.
- The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ — the values of the packets.

## Output Format
- Return a single integer — the maximum absolute difference.

## Constraints
- 1 ≤ n ≤ 1.5 * 10^5
- 1 ≤ a[i] ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, math, number-theory


