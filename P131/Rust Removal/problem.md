## Title
Rust Removal

## Slug
rust-removal

## Difficulty
Medium

## Description
A mechanic is sandblasting rust. The machine clears rust particles in counts matching the digits of the remaining rust estimate.

You start with a **rust amount** of `n`. The goal is to reduce this rust amount to exactly 0.

In one **blast**, you can look at the digits of the current rust amount, choose one **non-zero digit**, and subtract it from the current rust amount.

For example, if the rust amount is 27, the digits are 2 and 7. You can subtract 2 (getting 25) or 7 (getting 20).

Your task is to find the **minimum** number of blasts required to reduce the rust amount to 0.

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
Total blasts: 5.

### 2

#### Input
0

#### Output
0

#### Explanation
The rust amount is already 0.

## Input Format
- The input contains a single integer `n`.

## Output Format
- Return a single integer representing the minimum number of blasts.

## Constraints
- 0 ≤ n ≤ 10^6

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, greedy, math, bfs
