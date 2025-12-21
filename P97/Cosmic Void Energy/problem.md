## Title
Cosmic Void Energy

## Slug
cosmic-void-energy

## Difficulty
Hard

## Description
An astrophysicist detects a stream of cosmic rays. A stable energy pocket occurs when the total energy equals the missing quantum state.

Dr. Nova is analyzing a sequence of n energy bursts. Each burst has a specific intensity (a non-negative integer).

A contiguous group of energy bursts is considered **stable** if the sum of their intensity values is exactly equal to the **Void State** of that group.

The Void State (Minimum Excluded Value or MEX) is defined as the smallest non-negative integer that does not exist among the intensity values in the group.
For example:
- MEX of [1, 2] is 0
- MEX of [0, 2] is 1
- MEX of [0, 1, 2] is 3

Your task is to count the number of non-empty continuous subsegments that are stable.

## Examples

### 1

#### Input
5
0 1 2 0 1

#### Output
4

#### Explanation
The stable subsegments are:
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
- The first line contains a single integer $n$ — the number of energy bursts.
- The second line contains $n$ space-separated integers representing the intensity values.

## Output Format
- Return a single integer representing the number of stable subsegments.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ intensity ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
two-pointers, maths, array
