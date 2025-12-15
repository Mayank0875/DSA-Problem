## Title
Textile Dyeing

## Slug
textile-dyeing

## Difficulty
Hard

## Description
A fabric roll has `n` sections. It is cut into `k` pieces for dyeing. The 'dye absorption variance' for a piece is the square of its total length.

You must partition the sequence of sections into exactly `k` non-empty contiguous pieces.
Each piece corresponds to a vat.
The "absorption variance" for a vat is calculated as the **square of the sum** of the lengths of the sections in that piece.

Your goal is to minimize the total absorption variance (the sum of the absorption variance values of all `k` pieces).

## Examples

### 1

#### Input
8 3
2 3 1 2 2 3 4 1

#### Output
110

#### Explanation
We partition the sections into 3 pieces: `[2, 3, 1]`, `[2, 2, 3]`, and `[4, 1]`.
The sums are 6, 7, 5.
The total absorption variance is $6^2 + 7^2 + 5^2 = 36 + 49 + 25 = 110$.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
225

#### Explanation
Only 1 piece is allowed, containing all sections. Sum = 15. absorption variance = $15^2 = 225$.

## Input Format
- The first line contains two integers `n` and `k`: the number of sections and the required number of pieces.
- The second line contains `n` integers representing the lengths of each section.

## Output Format
- Return one integer: the minimum total absorption variance.

## Constraints
- 1 ≤ k ≤ n ≤ 3000
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, array
