## Title
Train Car Arrangement

## Slug
train-car-arrangement

## Difficulty
Hard

## Description
A train is assembled with numbered cars. For balance, no two cars with the same weight class (digit) are coupled directly together.

For example, the train configuration `12321` is valid because no two adjacent weight classes are the same. However, `1223` is invalid because the weight class `2` appears twice consecutively.

You are given a range of train configurations from $a$ to $b$ (inclusive). Your task is to calculate exactly how many train configurations in this range satisfy this condition.

## Examples

### 1

#### Input
123 321

#### Output
171

#### Explanation
There are 171 valid train configurations between 123 and 321 (inclusive).

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
- Return a single integer representing the count of valid train configurations in the range $[a, b]$.

## Constraints
- 0 ≤ a ≤ b ≤ 10^18

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, maths
