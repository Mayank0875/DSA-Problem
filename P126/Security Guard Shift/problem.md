## Title
Security Guard Shift

## Slug
security-guard-shift

## Difficulty
Easy

## Description
A secure facility tracks guard patrols.

The roster records the shift start and shift end of every guard in two integer arrays, `startTime` and `endTime`. The $i$-th guard clocks in at `startTime[i]` and clocks out at `endTime[i]`, inclusive.

The chief of security wants to know how many guards were on duty during a specific incident time `[queryStart, queryEnd]`. A guard is considered on duty if their patrol overlaps with the incident time at any point (even for a single moment).

Your task is to return the total number of guards who were on duty during the given incident time.

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
The incident time is `[2, 4]`.
- Guard 1 `[1, 3]` overlaps with `[2, 4]` (times 2, 3).
- Guard 2 `[2, 2]` overlaps with `[2, 4]` (time 2).
- Guard 3 `[3, 7]` overlaps with `[2, 4]` (times 3, 4).
All 3 guards were on duty.

### 2

#### Input
1
4
4
1 3

#### Output
0

#### Explanation
The guard was on duty at time `[4, 4]`. The incident time is `[1, 3]`. There is no overlap.

## Input Format
- The first line contains an integer `n`, the number of guards.
- The second line contains `n` space-separated integers for `startTime`.
- The third line contains `n` space-separated integers for `endTime`.
- The fourth line contains two integers, `queryStart` and `queryEnd`.

## Output Format
- Return a single integer representing the number of guards on duty during the incident time.

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
