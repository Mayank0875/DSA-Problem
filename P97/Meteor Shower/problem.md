## Title
Meteor Shower

## Slug
meteor-shower

## Difficulty
Hard

## Description
An astronomer tracks meteors. A cluster is 'rare' if the total mass equals the missing spectral type ID.

Stargazer is analyzing a sequence of n meteors. Each meteor has a specific mass index (a non-negative integer).

A contiguous group of meteors is considered **rare** if the sum of their mass index values is exactly equal to the **Dark Matter Type** of that group.

The Dark Matter Type (Minimum Excluded Value or MEX) is defined as the smallest non-negative integer that does not exist among the mass index values in the group.
For example:
- MEX of [1, 2] is 0
- MEX of [0, 2] is 1
- MEX of [0, 1, 2] is 3

Your task is to count the number of non-empty continuous subsegments that are rare.

## Examples

### 1

#### Input
5
0 1 2 0 1

#### Output
4

#### Explanation
The rare subsegments are:
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
- The first line contains a single integer $n$ — the number of meteors.
- The second line contains $n$ space-separated integers representing the mass index values.

## Output Format
- Return a single integer representing the number of rare subsegments.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ mass index ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
two-pointers, maths, array
