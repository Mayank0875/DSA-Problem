## Title
Chemical Isotope IDs

## Slug
chemical-isotope-ids

## Difficulty
Hard

## Description
Isotopes are cataloged by ID. Stable isotopes never have identifiers with repeating adjacent digits.

For example, the isotope ID `12321` is valid because no two adjacent digits are the same. However, `1223` is invalid because the digit `2` appears twice consecutively.

You are given a range of isotope IDs from $a$ to $b$ (inclusive). Your task is to calculate exactly how many isotope IDs in this range satisfy this condition.

## Examples

### 1

#### Input
123 321

#### Output
171

#### Explanation
There are 171 valid isotope IDs between 123 and 321 (inclusive).

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
- Return a single integer representing the count of valid isotope IDs in the range $[a, b]$.

## Constraints
- 0 ≤ a ≤ b ≤ 10^18

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, maths
