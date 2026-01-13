## Title
Candy Distribution

## Slug
candy-distribution

## Difficulty
Medium

## Description
A shopkeeper puts candies into gift bags.

The shopkeeper has prepared $n$ candies arranged in a sequence. The $i$-th candy has a value of $a_i$.

These candies need to be grouped into bags. Every bag must hold the exact same number of candies, denoted by $k$. The grouping happens sequentially:
- The first $k$ candies go into the first bag.
- The second $k$ candies go into the second bag.
- ...
- The last $k$ candies go into the $(n/k)$-th bag.

Since every bag must have exactly $k$ candies, this grouping is only possible if $n$ is divisible by $k$ ($1 \le k \le n$).

The shopkeeper wants to choose a valid $k$ such that the **difference between the maximum total value and the minimum total value** of the bags is maximized. If there is only one bag (i.e., $k=n$), the difference is 0.

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
- $k=1$: bag 1 has sum 1, bag 2 has sum 2. Difference = $|2-1| = 1$.
- $k=2$: Only one bag with sum $1+2=3$. Difference = 0.
Max difference is 1.

### 2

#### Input
4
10 10 10 10

#### Output
0

#### Explanation
All candies are equal. Regardless of $k$, all bags will have the same sum. Difference is always 0.

## Input Format
- The first line contains one integer $n$ — the number of candies.
- The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ — the values of the candies.

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


