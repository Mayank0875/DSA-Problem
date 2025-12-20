## Title
Music Melody Generation

## Slug
music-melody-generation

## Difficulty
Hard

## Description
An AI composes melodies represented by numbers. To avoid monotony, it never plays the same note (digit) twice consecutively.

For example, the melody `12321` is valid because no two adjacent notes are the same. However, `1223` is invalid because the note `2` appears twice consecutively.

You are given a range of melodies from $a$ to $b$ (inclusive). Your task is to calculate exactly how many melodies in this range satisfy this condition.

## Examples

### 1

#### Input
123 321

#### Output
171

#### Explanation
There are 171 valid melodies between 123 and 321 (inclusive).

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
- Return a single integer representing the count of valid melodies in the range $[a, b]$.

## Constraints
- 0 ≤ a ≤ b ≤ 10^18

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, maths
