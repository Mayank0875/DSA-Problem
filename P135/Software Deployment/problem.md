## Title
Software Deployment

## Slug
software-deployment

## Difficulty
Medium

## Description
A DevOps lead deploys microservices to nodes.

The lead has prepared $n$ services arranged in a sequence. The $i$-th service has a value of $a_i$.

These services need to be grouped into nodes. Every node must hold the exact same number of services, denoted by $k$. The grouping happens sequentially:
- The first $k$ services go into the first node.
- The second $k$ services go into the second node.
- ...
- The last $k$ services go into the $(n/k)$-th node.

Since every node must have exactly $k$ services, this grouping is only possible if $n$ is divisible by $k$ ($1 \le k \le n$).

The lead wants to choose a valid $k$ such that the **difference between the maximum total value and the minimum total value** of the nodes is maximized. If there is only one node (i.e., $k=n$), the difference is 0.

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
- $k=1$: node 1 has sum 1, node 2 has sum 2. Difference = $|2-1| = 1$.
- $k=2$: Only one node with sum $1+2=3$. Difference = 0.
Max difference is 1.

### 2

#### Input
4
10 10 10 10

#### Output
0

#### Explanation
All services are equal. Regardless of $k$, all nodes will have the same sum. Difference is always 0.

## Input Format
- The first line contains one integer $n$ — the number of services.
- The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ — the values of the services.

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


