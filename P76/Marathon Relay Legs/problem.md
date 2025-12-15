## Title
Marathon Relay Legs

## Slug
marathon-relay-legs

## Difficulty
Hard

## Description
A race course has `n` checkpoints with distances between them. A team of `k` runners splits the course. Each runner takes a contiguous section. The 'exhaustion' of a runner is the square of the distance they run.

You must partition the sequence of sections into exactly `k` non-empty contiguous legs.
Each leg corresponds to a runner.
The "exhaustion" for a runner is calculated as the **square of the sum** of the distances of the sections in that leg.

Your goal is to minimize the total exhaustion (the sum of the exhaustion values of all `k` legs).

## Examples

### 1

#### Input
8 3
2 3 1 2 2 3 4 1

#### Output
110

#### Explanation
We partition the sections into 3 legs: `[2, 3, 1]`, `[2, 2, 3]`, and `[4, 1]`.
The sums are 6, 7, 5.
The total exhaustion is $6^2 + 7^2 + 5^2 = 36 + 49 + 25 = 110$.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
225

#### Explanation
Only 1 leg is allowed, containing all sections. Sum = 15. exhaustion = $15^2 = 225$.

## Input Format
- The first line contains two integers `n` and `k`: the number of sections and the required number of legs.
- The second line contains `n` integers representing the distances of each section.

## Output Format
- Return one integer: the minimum total exhaustion.

## Constraints
- 1 ≤ k ≤ n ≤ 3000
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, array
