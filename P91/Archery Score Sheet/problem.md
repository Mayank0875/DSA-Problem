## Title
Archery Score Sheet

## Slug
archery-score-sheet

## Difficulty
Hard

## Description
Scores are recorded as a single long integer. A perfect sheet implies variety; no two adjacent shots scored the exact same digit value.

For example, the score sheet `12321` is valid because no two adjacent scores are the same. However, `1223` is invalid because the score `2` appears twice consecutively.

You are given a range of score sheets from $a$ to $b$ (inclusive). Your task is to calculate exactly how many score sheets in this range satisfy this condition.

## Examples

### 1

#### Input
123 321

#### Output
171

#### Explanation
There are 171 valid score sheets between 123 and 321 (inclusive).

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
- Return a single integer representing the count of valid score sheets in the range $[a, b]$.

## Constraints
- 0 ≤ a ≤ b ≤ 10^18

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, maths
