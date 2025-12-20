## Title
Color Coded Wires

## Slug
color-coded-wires

## Difficulty
Hard

## Description
Electricians identify wires by numeric color codes. A safe wire configuration never has adjacent bands of the same color code to prevent confusion.

For example, the wire code `12321` is valid because no two adjacent bands are the same. However, `1223` is invalid because the band `2` appears twice consecutively.

You are given a range of wire codes from $a$ to $b$ (inclusive). Your task is to calculate exactly how many wire codes in this range satisfy this condition.

## Examples

### 1

#### Input
123 321

#### Output
171

#### Explanation
There are 171 valid wire codes between 123 and 321 (inclusive).

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
- Return a single integer representing the count of valid wire codes in the range $[a, b]$.

## Constraints
- 0 ≤ a ≤ b ≤ 10^18

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, maths
