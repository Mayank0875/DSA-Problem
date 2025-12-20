## Title
Stuttering Robot

## Slug
stuttering-robot

## Difficulty
Hard

## Description
A robot is programmed to speak numbers, but it has a glitch where it sometimes repeats the same digit twice in a row (stuttering). A 'smooth' number is one where the robot does not stutter.

For example, the number `12321` is valid because no two adjacent digits are the same. However, `1223` is invalid because the digit `2` appears twice consecutively.

You are given a range of numbers from $a$ to $b$ (inclusive). Your task is to calculate exactly how many numbers in this range satisfy this condition.

## Examples

### 1

#### Input
123 321

#### Output
171

#### Explanation
There are 171 valid numbers between 123 and 321 (inclusive).

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
- Return a single integer representing the count of valid numbers in the range $[a, b]$.

## Constraints
- 0 ≤ a ≤ b ≤ 10^18

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, maths
