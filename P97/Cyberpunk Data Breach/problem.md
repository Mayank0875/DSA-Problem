## Title
Cyberpunk Data Breach

## Slug
cyberpunk-data-breach

## Difficulty
Hard

## Description
A hacker scans data packets. A breach creates a 'Ghost Protocol' if the checksum of the packet block equals the lowest missing protocol ID.

Neo is analyzing a sequence of n packets. Each packet has a specific ID value (a non-negative integer).

A contiguous group of packets is considered **compromised** if the sum of their ID value values is exactly equal to the **Ghost ID** of that group.

The Ghost ID (Minimum Excluded Value or MEX) is defined as the smallest non-negative integer that does not exist among the ID value values in the group.
For example:
- MEX of [1, 2] is 0
- MEX of [0, 2] is 1
- MEX of [0, 1, 2] is 3

Your task is to count the number of non-empty continuous subsegments that are compromised.

## Examples

### 1

#### Input
5
0 1 2 0 1

#### Output
4

#### Explanation
The compromised subsegments are:
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
- The first line contains a single integer $n$ — the number of packets.
- The second line contains $n$ space-separated integers representing the ID value values.

## Output Format
- Return a single integer representing the number of compromised subsegments.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ ID value ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
two-pointers, maths, array
