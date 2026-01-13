## Title
Server Load Balancing

## Slug
server-load-balancing

## Difficulty
Medium

## Description
A sysadmin assigns tasks to server clusters.

The sysadmin has prepared $n$ tasks arranged in a sequence. The $i$-th task has a value of $a_i$.

These tasks need to be grouped into clusters. Every cluster must hold the exact same number of tasks, denoted by $k$. The grouping happens sequentially:
- The first $k$ tasks go into the first cluster.
- The second $k$ tasks go into the second cluster.
- ...
- The last $k$ tasks go into the $(n/k)$-th cluster.

Since every cluster must have exactly $k$ tasks, this grouping is only possible if $n$ is divisible by $k$ ($1 \le k \le n$).

The sysadmin wants to choose a valid $k$ such that the **difference between the maximum total value and the minimum total value** of the clusters is maximized. If there is only one cluster (i.e., $k=n$), the difference is 0.

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
- $k=1$: cluster 1 has sum 1, cluster 2 has sum 2. Difference = $|2-1| = 1$.
- $k=2$: Only one cluster with sum $1+2=3$. Difference = 0.
Max difference is 1.

### 2

#### Input
4
10 10 10 10

#### Output
0

#### Explanation
All tasks are equal. Regardless of $k$, all clusters will have the same sum. Difference is always 0.

## Input Format
- The first line contains one integer $n$ — the number of tasks.
- The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ — the values of the tasks.

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


