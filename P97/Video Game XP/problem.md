## Title
Video Game XP

## Slug
video-game-xp

## Difficulty
Hard

## Description
A gamer grinds for XP. A level-up occurs if the total XP of a mob group equals the missing quest ID.

The Gamer is analyzing a sequence of n mobs. Each mob has a specific XP drop (a non-negative integer).

A contiguous group of mobs is considered **level-up** if the sum of their XP drop values is exactly equal to the **Hidden Quest** of that group.

The Hidden Quest (Minimum Excluded Value or MEX) is defined as the smallest non-negative integer that does not exist among the XP drop values in the group.
For example:
- MEX of [1, 2] is 0
- MEX of [0, 2] is 1
- MEX of [0, 1, 2] is 3

Your task is to count the number of non-empty continuous subsegments that are level-up.

## Examples

### 1

#### Input
5
0 1 2 0 1

#### Output
4

#### Explanation
The level-up subsegments are:
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
- The first line contains a single integer $n$ — the number of mobs.
- The second line contains $n$ space-separated integers representing the XP drop values.

## Output Format
- Return a single integer representing the number of level-up subsegments.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ XP drop ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
two-pointers, maths, array
