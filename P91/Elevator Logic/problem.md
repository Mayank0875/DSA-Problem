## Title
Elevator Logic

## Slug
elevator-logic

## Difficulty
Hard

## Description
A futuristic elevator uses a keypad. It ignores input if the user presses the same floor digit button twice in a row.

For example, the input sequence `12321` is valid because no two adjacent buttons are the same. However, `1223` is invalid because the button `2` appears twice consecutively.

You are given a range of input sequences from $a$ to $b$ (inclusive). Your task is to calculate exactly how many input sequences in this range satisfy this condition.

## Examples

### 1

#### Input
123 321

#### Output
171

#### Explanation
There are 171 valid input sequences between 123 and 321 (inclusive).

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
- Return a single integer representing the count of valid input sequences in the range $[a, b]$.

## Constraints
- 0 ≤ a ≤ b ≤ 10^18

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, maths
