## Title
Robot Vacuum Path

## Slug
robot-vacuum-path

## Difficulty
Hard

## Description
A robot vacuum stores its path as a numeric string. It is programmed to never make the exact same micro-movement (digit) twice in a row.

For example, the path string `12321` is valid because no two adjacent movements are the same. However, `1223` is invalid because the movement `2` appears twice consecutively.

You are given a range of path strings from $a$ to $b$ (inclusive). Your task is to calculate exactly how many path strings in this range satisfy this condition.

## Examples

### 1

#### Input
123 321

#### Output
171

#### Explanation
There are 171 valid path strings between 123 and 321 (inclusive).

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
- Return a single integer representing the count of valid path strings in the range $[a, b]$.

## Constraints
- 0 ≤ a ≤ b ≤ 10^18

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, maths
