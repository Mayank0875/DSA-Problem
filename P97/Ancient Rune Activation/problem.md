## Title
Ancient Rune Activation

## Slug
ancient-rune-activation

## Difficulty
Hard

## Description
An archaeologist studies a wall of runes. A spell activates if the total magic power of a sequence matches the forgotten rune symbol.

Indy is analyzing a sequence of n runes. Each rune has a specific power level (a non-negative integer).

A contiguous group of runes is considered **active** if the sum of their power level values is exactly equal to the **Forgotten Symbol** of that group.

The Forgotten Symbol (Minimum Excluded Value or MEX) is defined as the smallest non-negative integer that does not exist among the power level values in the group.
For example:
- MEX of [1, 2] is 0
- MEX of [0, 2] is 1
- MEX of [0, 1, 2] is 3

Your task is to count the number of non-empty continuous subsegments that are active.

## Examples

### 1

#### Input
5
0 1 2 0 1

#### Output
4

#### Explanation
The active subsegments are:
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
- The first line contains a single integer $n$ — the number of runes.
- The second line contains $n$ space-separated integers representing the power level values.

## Output Format
- Return a single integer representing the number of active subsegments.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ power level ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
two-pointers, maths, array
