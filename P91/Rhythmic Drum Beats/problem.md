## Title
Rhythmic Drum Beats

## Slug
rhythmic-drum-beats

## Difficulty
Hard

## Description
A drummer uses a number notation for beats. To keep the rhythm dynamic, he avoids playing the exact same beat type twice in a row.

For example, the beat pattern `12321` is valid because no two adjacent beat types are the same. However, `1223` is invalid because the beat type `2` appears twice consecutively.

You are given a range of beat patterns from $a$ to $b$ (inclusive). Your task is to calculate exactly how many beat patterns in this range satisfy this condition.

## Examples

### 1

#### Input
123 321

#### Output
171

#### Explanation
There are 171 valid beat patterns between 123 and 321 (inclusive).

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
- Return a single integer representing the count of valid beat patterns in the range $[a, b]$.

## Constraints
- 0 ≤ a ≤ b ≤ 10^18

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, maths
