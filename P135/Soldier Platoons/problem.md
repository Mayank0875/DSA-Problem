## Title
Soldier Platoons

## Slug
soldier-platoons

## Difficulty
Medium

## Description
A general organizes soldiers into platoons.

The general has prepared $n$ soldiers arranged in a sequence. The $i$-th soldier has a value of $a_i$.

These soldiers need to be grouped into platoons. Every platoon must hold the exact same number of soldiers, denoted by $k$. The grouping happens sequentially:
- The first $k$ soldiers go into the first platoon.
- The second $k$ soldiers go into the second platoon.
- ...
- The last $k$ soldiers go into the $(n/k)$-th platoon.

Since every platoon must have exactly $k$ soldiers, this grouping is only possible if $n$ is divisible by $k$ ($1 \le k \le n$).

The general wants to choose a valid $k$ such that the **difference between the maximum total value and the minimum total value** of the platoons is maximized. If there is only one platoon (i.e., $k=n$), the difference is 0.

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
- $k=1$: platoon 1 has sum 1, platoon 2 has sum 2. Difference = $|2-1| = 1$.
- $k=2$: Only one platoon with sum $1+2=3$. Difference = 0.
Max difference is 1.

### 2

#### Input
4
10 10 10 10

#### Output
0

#### Explanation
All soldiers are equal. Regardless of $k$, all platoons will have the same sum. Difference is always 0.

## Input Format
- The first line contains one integer $n$ — the number of soldiers.
- The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ — the values of the soldiers.

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


