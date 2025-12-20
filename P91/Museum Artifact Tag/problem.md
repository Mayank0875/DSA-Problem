## Title
Museum Artifact Tag

## Slug
museum-artifact-tag

## Difficulty
Hard

## Description
Artifacts are tagged. The curator demands tags be 'aesthetically pleasing', which defined as having no adjacent duplicate figures.

For example, the tag `12321` is valid because no two adjacent figures are the same. However, `1223` is invalid because the figure `2` appears twice consecutively.

You are given a range of tags from $a$ to $b$ (inclusive). Your task is to calculate exactly how many tags in this range satisfy this condition.

## Examples

### 1

#### Input
123 321

#### Output
171

#### Explanation
There are 171 valid tags between 123 and 321 (inclusive).

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
- Return a single integer representing the count of valid tags in the range $[a, b]$.

## Constraints
- 0 ≤ a ≤ b ≤ 10^18

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, maths
