## Title
Forest Planting

## Slug
forest-planting

## Difficulty
Medium

## Description
A ranger plants trees. Oaks (0) are planted in the first sector, Pines (1) in the second.

We can represent the arrangement as a binary string `forest` of length `n`, consisting of '0's (Oaks) and '1's (Pines). A string is considered **sorted** if all '0's appear before all '1's.

You possess a specific technique to organize them. In one operation, you can:
1. Choose any substring of `forest`.
2. Choose a positive integer `k`.
3. Cyclically shift the chosen substring to the left by `k` positions.

For example, shifting the substring `1011` of string `0101100` by 2 positions results in `0111000`.

Your task is to calculate the **minimum number of operations** required to make the string `forest` sorted (i.e., all Oakss precede all Piness).

## Examples

### 1

#### Input
01010101

#### Output
3

#### Explanation
We need to move the Oakss (0) that appear after Piness (1).
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
There are three distinct groups of '0's (Oaks) that appear after the first '1' (Pines):
1. The group `00` at indices 2-3.
2. The group `0` at index 5.
3. The group `000` at indices 7-9.
Each group requires one operation.

## Input Format
- The first line contains a single string `forest` consisting only of characters '0' and '1'.

## Output Format
- Return a single integer representing the minimum number of operations required.

## Constraints
- 1 ≤ forest.length ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy
