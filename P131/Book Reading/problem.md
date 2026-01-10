## Title
Book Reading

## Slug
book-reading

## Difficulty
Medium

## Description
A speed reader finishes pages. They read a chunk of pages equal to a digit of the number of pages left.

You start with a **pages left** of `n`. The goal is to reduce this pages left to exactly 0.

In one **reading session**, you can look at the digits of the current pages left, choose one **non-zero digit**, and subtract it from the current pages left.

For example, if the pages left is 27, the digits are 2 and 7. You can subtract 2 (getting 25) or 7 (getting 20).

Your task is to find the **minimum** number of reading sessions required to reduce the pages left to 0.

## Examples

### 1

#### Input
27

#### Output
5

#### Explanation
1. 27 - 7 = 20
2. 20 - 2 = 18
3. 18 - 8 = 10
4. 10 - 1 = 9
5. 9 - 9 = 0
Total reading sessions: 5.

### 2

#### Input
0

#### Output
0

#### Explanation
The pages left is already 0.

## Input Format
- The input contains a single integer `n`.

## Output Format
- Return a single integer representing the minimum number of reading sessions.

## Constraints
- 0 ≤ n ≤ 10^6

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, greedy, math, bfs
