## Title
Weather Storm Duration

## Slug
weather-storm-duration

## Difficulty
Easy

## Description
Meteorologists track storms passing through a region.

The radar history records the storm start and storm end of every storm in two integer arrays, `startTime` and `endTime`. The $i$-th storm forms at `startTime[i]` and dissipates at `endTime[i]`, inclusive.

The weatherman wants to know how many storms were active during a specific alert period `[queryStart, queryEnd]`. A storm is considered active if their life cycle overlaps with the alert period at any point (even for a single moment).

Your task is to return the total number of storms who were active during the given alert period.

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
The alert period is `[2, 4]`.
- Storm 1 `[1, 3]` overlaps with `[2, 4]` (times 2, 3).
- Storm 2 `[2, 2]` overlaps with `[2, 4]` (time 2).
- Storm 3 `[3, 7]` overlaps with `[2, 4]` (times 3, 4).
All 3 storms were active.

### 2

#### Input
1
4
4
1 3

#### Output
0

#### Explanation
The storm was active at time `[4, 4]`. The alert period is `[1, 3]`. There is no overlap.

## Input Format
- The first line contains an integer `n`, the number of storms.
- The second line contains `n` space-separated integers for `startTime`.
- The third line contains `n` space-separated integers for `endTime`.
- The fourth line contains two integers, `queryStart` and `queryEnd`.

## Output Format
- Return a single integer representing the number of storms active during the alert period.

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
