## Title
Space Travel

## Slug
space-travel

## Difficulty
Hard

## Description
A navigator plots a course. A sector is 'passable' if the total star mass equals the missing gravity well constant.

Navigator is analyzing a sequence of n stars. Each star has a specific mass (a non-negative integer).

A contiguous group of stars is considered **passable** if the sum of their mass values is exactly equal to the **Dark Gravity** of that group.

The Dark Gravity (Minimum Excluded Value or MEX) is defined as the smallest non-negative integer that does not exist among the mass values in the group.
For example:
- MEX of [1, 2] is 0
- MEX of [0, 2] is 1
- MEX of [0, 1, 2] is 3

Your task is to count the number of non-empty continuous subsegments that are passable.

## Examples

### 1

#### Input
5
0 1 2 0 1

#### Output
4

#### Explanation
The passable subsegments are:
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
- The first line contains a single integer $n$ — the number of stars.
- The second line contains $n$ space-separated integers representing the mass values.

## Output Format
- Return a single integer representing the number of passable subsegments.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ mass ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
two-pointers, maths, array
