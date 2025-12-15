## Title
Exam Grading Piles

## Slug
exam-grading-piles

## Difficulty
Hard

## Description
A professor divides `n` exam papers among `k` teaching assistants. Papers vary in complexity. They are split into contiguous piles from the stack. The 'grading fatigue' for a TA is the square of the total complexity of their pile.

You must partition the sequence of papers into exactly `k` non-empty contiguous piles.
Each pile corresponds to a TA.
The "grading fatigue" for a TA is calculated as the **square of the sum** of the complexity scores of the papers in that pile.

Your goal is to minimize the total grading fatigue (the sum of the grading fatigue values of all `k` piles).

## Examples

### 1

#### Input
8 3
2 3 1 2 2 3 4 1

#### Output
110

#### Explanation
We partition the papers into 3 piles: `[2, 3, 1]`, `[2, 2, 3]`, and `[4, 1]`.
The sums are 6, 7, 5.
The total grading fatigue is $6^2 + 7^2 + 5^2 = 36 + 49 + 25 = 110$.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
225

#### Explanation
Only 1 pile is allowed, containing all papers. Sum = 15. grading fatigue = $15^2 = 225$.

## Input Format
- The first line contains two integers `n` and `k`: the number of papers and the required number of piles.
- The second line contains `n` integers representing the complexity scores of each paper.

## Output Format
- Return one integer: the minimum total grading fatigue.

## Constraints
- 1 ≤ k ≤ n ≤ 3000
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, array
