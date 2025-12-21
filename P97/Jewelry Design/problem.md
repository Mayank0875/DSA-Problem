## Title
Jewelry Design

## Slug
jewelry-design

## Difficulty
Hard

## Description
A jeweler sets stones. A necklace is 'masterpiece' if the total carat weight equals the missing gem type.

The Jeweler is analyzing a sequence of n stones. Each stone has a specific carats (a non-negative integer).

A contiguous group of stones is considered **masterpiece** if the sum of their carats values is exactly equal to the **Rare Gem** of that group.

The Rare Gem (Minimum Excluded Value or MEX) is defined as the smallest non-negative integer that does not exist among the carats values in the group.
For example:
- MEX of [1, 2] is 0
- MEX of [0, 2] is 1
- MEX of [0, 1, 2] is 3

Your task is to count the number of non-empty continuous subsegments that are masterpiece.

## Examples

### 1

#### Input
5
0 1 2 0 1

#### Output
4

#### Explanation
The masterpiece subsegments are:
- `[0, 1, 2]` (Indices 0-2): Sum = 3, MEX = 3.
- `[1, 2, 0]` (Indices 1-3): Sum = 3, MEX = 3.
- `[2, 0, 1]` (Indices 2-4): Sum = 3, MEX = 3.
- `[0, 1, 2, 0]` (Indices 0-3): Sum = 3, MEX = 3.

### 2

#### Input
3
1 1 1

#### Output
0

#### Explanation
No subsegment satisfies the condition. For `[1]`, Sum=1, MEX=0.

## Input Format
- The first line contains a single integer $n$ — the number of stones.
- The second line contains $n$ space-separated integers representing the carats values.

## Output Format
- Return a single integer representing the number of masterpiece subsegments.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ carats ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
two-pointers, maths, array
