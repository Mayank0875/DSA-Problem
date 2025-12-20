## Title
Digital Art Pixels

## Slug
digital-art-pixels

## Difficulty
Hard

## Description
An artist creates numeric art. They have a rule: no two pixels in a row (digits) can have the same color value.

For example, the row value `12321` is valid because no two adjacent pixels are the same. However, `1223` is invalid because the pixel `2` appears twice consecutively.

You are given a range of row values from $a$ to $b$ (inclusive). Your task is to calculate exactly how many row values in this range satisfy this condition.

## Examples

### 1

#### Input
123 321

#### Output
171

#### Explanation
There are 171 valid row values between 123 and 321 (inclusive).

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
- Return a single integer representing the count of valid row values in the range $[a, b]$.

## Constraints
- 0 ≤ a ≤ b ≤ 10^18

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, maths
