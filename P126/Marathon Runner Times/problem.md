## Title
Marathon Runner Times

## Slug
marathon-runner-times

## Difficulty
Easy

## Description
A race tracks runners on a specific segment of the course.

The chip timer records the segment start time and segment end time of every runner in two integer arrays, `startTime` and `endTime`. The $i$-th runner enters the segment at `startTime[i]` and leaves the segment at `endTime[i]`, inclusive.

The race director wants to know how many runners were on the segment during a specific broadcast window `[queryStart, queryEnd]`. A runner is considered on the segment if their split overlaps with the broadcast window at any point (even for a single moment).

Your task is to return the total number of runners who were on the segment during the given broadcast window.

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
The broadcast window is `[2, 4]`.
- Runner 1 `[1, 3]` overlaps with `[2, 4]` (times 2, 3).
- Runner 2 `[2, 2]` overlaps with `[2, 4]` (time 2).
- Runner 3 `[3, 7]` overlaps with `[2, 4]` (times 3, 4).
All 3 runners were on the segment.

### 2

#### Input
1
4
4
1 3

#### Output
0

#### Explanation
The runner was on the segment at time `[4, 4]`. The broadcast window is `[1, 3]`. There is no overlap.

## Input Format
- The first line contains an integer `n`, the number of runners.
- The second line contains `n` space-separated integers for `startTime`.
- The third line contains `n` space-separated integers for `endTime`.
- The fourth line contains two integers, `queryStart` and `queryEnd`.

## Output Format
- Return a single integer representing the number of runners on the segment during the broadcast window.

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
