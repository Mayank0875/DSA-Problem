## Title
Team Balancing

## Slug
team-balancing

## Difficulty
Medium

## Description
A coach divides players into teams of equal size based on skill points.

The coach has prepared $n$ players arranged in a sequence. The $i$-th player has a value of $a_i$.

These players need to be grouped into teams. Every team must hold the exact same number of players, denoted by $k$. The grouping happens sequentially:
- The first $k$ players go into the first team.
- The second $k$ players go into the second team.
- ...
- The last $k$ players go into the $(n/k)$-th team.

Since every team must have exactly $k$ players, this grouping is only possible if $n$ is divisible by $k$ ($1 \le k \le n$).

The coach wants to choose a valid $k$ such that the **difference between the maximum total value and the minimum total value** of the teams is maximized. If there is only one team (i.e., $k=n$), the difference is 0.

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
- $k=1$: team 1 has sum 1, team 2 has sum 2. Difference = $|2-1| = 1$.
- $k=2$: Only one team with sum $1+2=3$. Difference = 0.
Max difference is 1.

### 2

#### Input
4
10 10 10 10

#### Output
0

#### Explanation
All players are equal. Regardless of $k$, all teams will have the same sum. Difference is always 0.

## Input Format
- The first line contains one integer $n$ — the number of players.
- The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ — the values of the players.

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


