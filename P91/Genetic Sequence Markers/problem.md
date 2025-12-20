## Title
Genetic Sequence Markers

## Slug
genetic-sequence-markers

## Difficulty
Hard

## Description
Synthetic biologists use numeric markers to tag genes. A stable marker must not have identical adjacent values, as this causes binding errors.

For example, the marker `12321` is valid because no two adjacent values are the same. However, `1223` is invalid because the value `2` appears twice consecutively.

You are given a range of markers from $a$ to $b$ (inclusive). Your task is to calculate exactly how many markers in this range satisfy this condition.

## Examples

### 1

#### Input
123 321

#### Output
171

#### Explanation
There are 171 valid markers between 123 and 321 (inclusive).

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
- Return a single integer representing the count of valid markers in the range $[a, b]$.

## Constraints
- 0 ≤ a ≤ b ≤ 10^18

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, maths
