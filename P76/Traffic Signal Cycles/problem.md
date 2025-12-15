## Title
Traffic Signal Cycles

## Slug
traffic-signal-cycles

## Difficulty
Hard

## Description
A smart traffic light manages `n` cars in a queue over `k` green light cycles. Each car has a delay factor. Cars pass in contiguous groups. The 'congestion penalty' for a cycle is the square of the total delay factor of cars clearing that cycle.

You must partition the sequence of cars into exactly `k` non-empty contiguous cycles.
Each cycle corresponds to a green light cycle.
The "congestion penalty" for a green light cycle is calculated as the **square of the sum** of the delay factors of the cars in that cycle.

Your goal is to minimize the total congestion penalty (the sum of the congestion penalty values of all `k` cycles).

## Examples

### 1

#### Input
8 3
2 3 1 2 2 3 4 1

#### Output
110

#### Explanation
We partition the cars into 3 cycles: `[2, 3, 1]`, `[2, 2, 3]`, and `[4, 1]`.
The sums are 6, 7, 5.
The total congestion penalty is $6^2 + 7^2 + 5^2 = 36 + 49 + 25 = 110$.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
225

#### Explanation
Only 1 cycle is allowed, containing all cars. Sum = 15. congestion penalty = $15^2 = 225$.

## Input Format
- The first line contains two integers `n` and `k`: the number of cars and the required number of cycles.
- The second line contains `n` integers representing the delay factors of each car.

## Output Format
- Return one integer: the minimum total congestion penalty.

## Constraints
- 1 ≤ k ≤ n ≤ 3000
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, array
