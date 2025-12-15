## Title
Fireworks Display

## Slug
fireworks-display

## Difficulty
Hard

## Description
A show has `n` fireworks shells. They are fired in `k` sequences. The 'smoke density' produced by a sequence is the square of the total gunpowder mass in that sequence.

You must partition the sequence of shells into exactly `k` non-empty contiguous sequences.
Each sequence corresponds to a sequence.
The "smoke density" for a sequence is calculated as the **square of the sum** of the gunpowder masses of the shells in that sequence.

Your goal is to minimize the total smoke density (the sum of the smoke density values of all `k` sequences).

## Examples

### 1

#### Input
8 3
2 3 1 2 2 3 4 1

#### Output
110

#### Explanation
We partition the shells into 3 sequences: `[2, 3, 1]`, `[2, 2, 3]`, and `[4, 1]`.
The sums are 6, 7, 5.
The total smoke density is $6^2 + 7^2 + 5^2 = 36 + 49 + 25 = 110$.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
225

#### Explanation
Only 1 sequence is allowed, containing all shells. Sum = 15. smoke density = $15^2 = 225$.

## Input Format
- The first line contains two integers `n` and `k`: the number of shells and the required number of sequences.
- The second line contains `n` integers representing the gunpowder masses of each shell.

## Output Format
- Return one integer: the minimum total smoke density.

## Constraints
- 1 ≤ k ≤ n ≤ 3000
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, array
