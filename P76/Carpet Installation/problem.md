## Title
Carpet Installation

## Slug
carpet-installation

## Difficulty
Hard

## Description
A hallway requires `n` strips of carpet. `k` installers work on contiguous sections. The 'glue usage rate' for a section is the square of the total area covered.

You must partition the sequence of strips into exactly `k` non-empty contiguous sections.
Each section corresponds to a installer.
The "glue usage rate" for a installer is calculated as the **square of the sum** of the areas of the strips in that section.

Your goal is to minimize the total glue usage rate (the sum of the glue usage rate values of all `k` sections).

## Examples

### 1

#### Input
8 3
2 3 1 2 2 3 4 1

#### Output
110

#### Explanation
We partition the strips into 3 sections: `[2, 3, 1]`, `[2, 2, 3]`, and `[4, 1]`.
The sums are 6, 7, 5.
The total glue usage rate is $6^2 + 7^2 + 5^2 = 36 + 49 + 25 = 110$.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
225

#### Explanation
Only 1 section is allowed, containing all strips. Sum = 15. glue usage rate = $15^2 = 225$.

## Input Format
- The first line contains two integers `n` and `k`: the number of strips and the required number of sections.
- The second line contains `n` integers representing the areas of each strip.

## Output Format
- Return one integer: the minimum total glue usage rate.

## Constraints
- 1 ≤ k ≤ n ≤ 3000
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, array
