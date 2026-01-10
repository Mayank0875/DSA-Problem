## Title
Museum Tour Groups

## Slug
museum-tour-groups

## Difficulty
Easy

## Description
A museum logs group entry and exit times.

The ticket scanner records the entry time and exit time of every group in two integer arrays, `startTime` and `endTime`. The $i$-th group enters at `startTime[i]` and leaves at `endTime[i]`, inclusive.

The curator wants to know how many groups were touring during a specific special exhibit hour `[queryStart, queryEnd]`. A group is considered touring if their visit overlaps with the special exhibit hour at any point (even for a single moment).

Your task is to return the total number of groups who were touring during the given special exhibit hour.

## Examples

### 1

#### Input
3
1 2 3
3 2 7
2 4

#### Output
3

#### Explanation
The special exhibit hour is `[2, 4]`.
- Group 1 `[1, 3]` overlaps with `[2, 4]` (times 2, 3).
- Group 2 `[2, 2]` overlaps with `[2, 4]` (time 2).
- Group 3 `[3, 7]` overlaps with `[2, 4]` (times 3, 4).
All 3 groups were touring.

### 2

#### Input
1
4
4
1 3

#### Output
0

#### Explanation
The group was touring at time `[4, 4]`. The special exhibit hour is `[1, 3]`. There is no overlap.

## Input Format
- The first line contains an integer `n`, the number of groups.
- The second line contains `n` space-separated integers for `startTime`.
- The third line contains `n` space-separated integers for `endTime`.
- The fourth line contains two integers, `queryStart` and `queryEnd`.

## Output Format
- Return a single integer representing the number of groups touring during the special exhibit hour.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ startTime[i] ≤ endTime[i] ≤ 10^9
- 1 ≤ queryStart ≤ queryEnd ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, interval, linear-scan

## Company
amazon
