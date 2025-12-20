## Title
Textile Pattern Code

## Slug
textile-pattern-code

## Difficulty
Hard

## Description
Weaving machines read numeric patterns. Repeating the same thread code twice in a row causes the machine to jam.

For example, the pattern code `12321` is valid because no two adjacent thread codes are the same. However, `1223` is invalid because the thread code `2` appears twice consecutively.

You are given a range of pattern codes from $a$ to $b$ (inclusive). Your task is to calculate exactly how many pattern codes in this range satisfy this condition.

## Examples

### 1

#### Input
123 321

#### Output
171

#### Explanation
There are 171 valid pattern codes between 123 and 321 (inclusive).

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
- Return a single integer representing the count of valid pattern codes in the range $[a, b]$.

## Constraints
- 0 ≤ a ≤ b ≤ 10^18

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, maths
