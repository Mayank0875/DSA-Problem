## Title
Traffic Flow Control

## Slug
traffic-flow-control

## Difficulty
Hard

## Description
A traffic controller watches car speeds. A flow block is 'smooth' if the total speed sum matches the lowest missing speed bracket.

Officer Judy is analyzing a sequence of n cars. Each car has a specific speed code (a non-negative integer).

A contiguous group of cars is considered **smooth** if the sum of their speed code values is exactly equal to the **Missing Speed** of that group.

The Missing Speed (Minimum Excluded Value or MEX) is defined as the smallest non-negative integer that does not exist among the speed code values in the group.
For example:
- MEX of [1, 2] is 0
- MEX of [0, 2] is 1
- MEX of [0, 1, 2] is 3

Your task is to count the number of non-empty continuous subsegments that are smooth.

## Examples

### 1

#### Input
5
0 1 2 0 1

#### Output
4

#### Explanation
The smooth subsegments are:
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
- The first line contains a single integer $n$ — the number of cars.
- The second line contains $n$ space-separated integers representing the speed code values.

## Output Format
- Return a single integer representing the number of smooth subsegments.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ speed code ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
two-pointers, maths, array
