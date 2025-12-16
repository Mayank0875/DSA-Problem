## Title
Cinema Seating

## Slug
cinema-seating

## Difficulty
Medium

## Description
An usher is organizing a row. VIP guests (0) should be seated to the left of Regular guests (1).

We can represent the arrangement as a binary string `row` of length `n`, consisting of '0's (VIP guests) and '1's (Regular guests). A string is considered **sorted** if all '0's appear before all '1's.

You possess a specific technique to organize them. In one operation, you can:
1. Choose any substring of `row`.
2. Choose a positive integer `k`.
3. Cyclically shift the chosen substring to the left by `k` positions.

For example, shifting the substring `1011` of string `0101100` by 2 positions results in `0111000`.

Your task is to calculate the **minimum number of operations** required to make the string `row` sorted (i.e., all VIP guestss precede all Regular guestss).

## Examples

### 1

#### Input
01010101

#### Output
3

#### Explanation
We need to move the VIP guestss (0) that appear after Regular guestss (1).
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
There are three distinct groups of '0's (VIP guests) that appear after the first '1' (Regular guests):
1. The group `00` at indices 2-3.
2. The group `0` at index 5.
3. The group `000` at indices 7-9.
Each group requires one operation.

## Input Format
- The first line contains a single string `row` consisting only of characters '0' and '1'.

## Output Format
- Return a single integer representing the minimum number of operations required.

## Constraints
- 1 ≤ row.length ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy
