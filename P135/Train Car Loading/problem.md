## Title
Train Car Loading

## Slug
train-car-loading

## Difficulty
Medium

## Description
A station master loads passengers into train cars.

The station master has prepared $n$ passengers arranged in a sequence. The $i$-th passenger group has a value of $a_i$.

These passengers need to be grouped into cars. Every car must hold the exact same number of passengers, denoted by $k$. The grouping happens sequentially:
- The first $k$ passengers go into the first car.
- The second $k$ passengers go into the second car.
- ...
- The last $k$ passengers go into the $(n/k)$-th car.

Since every car must have exactly $k$ passengers, this grouping is only possible if $n$ is divisible by $k$ ($1 \le k \le n$).

The station master wants to choose a valid $k$ such that the **difference between the maximum total value and the minimum total value** of the cars is maximized. If there is only one car (i.e., $k=n$), the difference is 0.

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
- $k=1$: car 1 has sum 1, car 2 has sum 2. Difference = $|2-1| = 1$.
- $k=2$: Only one car with sum $1+2=3$. Difference = 0.
Max difference is 1.

### 2

#### Input
4
10 10 10 10

#### Output
0

#### Explanation
All passengers are equal. Regardless of $k$, all cars will have the same sum. Difference is always 0.

## Input Format
- The first line contains one integer $n$ — the number of passengers.
- The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ — the values of the passengers.

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


