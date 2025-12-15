## Title
Painting Wall Sections

## Slug
painting-wall-sections

## Difficulty
Hard

## Description
A long wall is marked into `n` sections. `k` painters paint contiguous strips. The 'fume concentration' for a painter's area is the square of the total surface area they paint.

You must partition the sequence of sections into exactly `k` non-empty contiguous strips.
Each strip corresponds to a painter.
The "fume concentration" for a painter is calculated as the **square of the sum** of the areas of the sections in that strip.

Your goal is to minimize the total fume concentration (the sum of the fume concentration values of all `k` strips).

## Examples

### 1

#### Input
8 3
2 3 1 2 2 3 4 1

#### Output
110

#### Explanation
We partition the sections into 3 strips: `[2, 3, 1]`, `[2, 2, 3]`, and `[4, 1]`.
The sums are 6, 7, 5.
The total fume concentration is $6^2 + 7^2 + 5^2 = 36 + 49 + 25 = 110$.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
225

#### Explanation
Only 1 strip is allowed, containing all sections. Sum = 15. fume concentration = $15^2 = 225$.

## Input Format
- The first line contains two integers `n` and `k`: the number of sections and the required number of strips.
- The second line contains `n` integers representing the areas of each section.

## Output Format
- Return one integer: the minimum total fume concentration.

## Constraints
- 1 ≤ k ≤ n ≤ 3000
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, array
