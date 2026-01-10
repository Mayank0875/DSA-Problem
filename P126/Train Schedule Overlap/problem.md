## Title
Train Schedule Overlap

## Slug
train-schedule-overlap

## Difficulty
Easy

## Description
A railway station monitors train platform occupancy.

The platform log records the arrival time and departure time of every train in two integer arrays, `startTime` and `endTime`. The $i$-th train arrives at `startTime[i]` and departs at `endTime[i]`, inclusive.

The station master wants to know how many trains were at the platform during a specific rush hour window `[queryStart, queryEnd]`. A train is considered at the platform if their stop overlaps with the rush hour window at any point (even for a single moment).

Your task is to return the total number of trains who were at the platform during the given rush hour window.

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
The rush hour window is `[2, 4]`.
- Train 1 `[1, 3]` overlaps with `[2, 4]` (times 2, 3).
- Train 2 `[2, 2]` overlaps with `[2, 4]` (time 2).
- Train 3 `[3, 7]` overlaps with `[2, 4]` (times 3, 4).
All 3 trains were at the platform.

### 2

#### Input
1
4
4
1 3

#### Output
0

#### Explanation
The train was at the platform at time `[4, 4]`. The rush hour window is `[1, 3]`. There is no overlap.

## Input Format
- The first line contains an integer `n`, the number of trains.
- The second line contains `n` space-separated integers for `startTime`.
- The third line contains `n` space-separated integers for `endTime`.
- The fourth line contains two integers, `queryStart` and `queryEnd`.

## Output Format
- Return a single integer representing the number of trains at the platform during the rush hour window.

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
