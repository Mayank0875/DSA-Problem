## Title
Phone Number Allocation

## Slug
phone-number-allocation

## Difficulty
Hard

## Description
A telecom provider releases a premium batch of phone numbers. Premium numbers in this specific set must not have any repeating adjacent digits.

For example, the phone number `12321` is valid because no two adjacent digits are the same. However, `1223` is invalid because the digit `2` appears twice consecutively.

You are given a range of phone numbers from $a$ to $b$ (inclusive). Your task is to calculate exactly how many phone numbers in this range satisfy this condition.

## Examples

### 1

#### Input
123 321

#### Output
171

#### Explanation
There are 171 valid phone numbers between 123 and 321 (inclusive).

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
- Return a single integer representing the count of valid phone numbers in the range $[a, b]$.

## Constraints
- 0 ≤ a ≤ b ≤ 10^18

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, maths
