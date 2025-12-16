## Title
Construction Site

## Slug
construction-site

## Difficulty
Medium

## Description
Workers stack materials. Bricks (0) are used first, so they go before Wood (1).

We can represent the arrangement as a binary string `stack` of length `n`, consisting of '0's (Bricks) and '1's (Wood). A string is considered **sorted** if all '0's appear before all '1's.

You possess a specific technique to organize them. In one operation, you can:
1. Choose any substring of `stack`.
2. Choose a positive integer `k`.
3. Cyclically shift the chosen substring to the left by `k` positions.

For example, shifting the substring `1011` of string `0101100` by 2 positions results in `0111000`.

Your task is to calculate the **minimum number of operations** required to make the string `stack` sorted (i.e., all Brickss precede all Woods).

## Examples

### 1

#### Input
01010101

#### Output
3

#### Explanation
We need to move the Brickss (0) that appear after Woods (1).
There are three distinct groups of '0's appearing after the first '1'.
1. The '0' at index 2.
2. The '0' at index 4.
3. The '0' at index 6.
Each group requires one operation to effectively move to the correct side.

### 2

#### Input
11001010001

#### Output
3

#### Explanation
There are three distinct groups of '0's (Bricks) that appear after the first '1' (Wood):
1. The group `00` at indices 2-3.
2. The group `0` at index 5.
3. The group `000` at indices 7-9.
Each group requires one operation.

## Input Format
- The first line contains a single string `stack` consisting only of characters '0' and '1'.

## Output Format
- Return a single integer representing the minimum number of operations required.

## Constraints
- 1 ≤ stack.length ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy
