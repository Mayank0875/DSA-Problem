## Title
File System

## Slug
file-system

## Difficulty
Medium

## Description
An OS organizes files. System files (0) must remain at the start of the sector, followed by User files (1).

We can represent the arrangement as a binary string `sector` of length `n`, consisting of '0's (System files) and '1's (User files). A string is considered **sorted** if all '0's appear before all '1's.

You possess a specific technique to organize them. In one operation, you can:
1. Choose any substring of `sector`.
2. Choose a positive integer `k`.
3. Cyclically shift the chosen substring to the left by `k` positions.

For example, shifting the substring `1011` of string `0101100` by 2 positions results in `0111000`.

Your task is to calculate the **minimum number of operations** required to make the string `sector` sorted (i.e., all System filess precede all User filess).

## Examples

### 1

#### Input
01010101

#### Output
3

#### Explanation
We need to move the System filess (0) that appear after User filess (1).
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
There are three distinct groups of '0's (System files) that appear after the first '1' (User files):
1. The group `00` at indices 2-3.
2. The group `0` at index 5.
3. The group `000` at indices 7-9.
Each group requires one operation.

## Input Format
- The first line contains a single string `sector` consisting only of characters '0' and '1'.

## Output Format
- Return a single integer representing the minimum number of operations required.

## Constraints
- 1 ≤ sector.length ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy
