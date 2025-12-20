## Title
Safe Combination Design

## Slug
safe-combination-design

## Difficulty
Hard

## Description
A lock manufacturer claims their safes are harder to crack because the combination never uses the same number twice in a row, forcing the dial to always move.

For example, the combination `12321` is valid because no two adjacent numbers are the same. However, `1223` is invalid because the number `2` appears twice consecutively.

You are given a range of combinations from $a$ to $b$ (inclusive). Your task is to calculate exactly how many combinations in this range satisfy this condition.

## Examples

### 1

#### Input
123 321

#### Output
171

#### Explanation
There are 171 valid combinations between 123 and 321 (inclusive).

### 2

#### Input
1234 1234

#### Output
1

#### Explanation
The number 1234 is valid.

## Input Format
- The input contains two space-separated integers, $a$ and $b$.

## Output Format
- Return a single integer representing the count of valid combinations in the range $[a, b]$.

## Constraints
- 0 ≤ a ≤ b ≤ 10^18

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, maths
