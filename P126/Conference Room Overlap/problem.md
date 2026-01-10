## Title
Conference Room Overlap

## Slug
conference-room-overlap

## Difficulty
Easy

## Description
A corporate office tracks meeting room usage.

The scheduling system records the start time and end time of every meeting in two integer arrays, `startTime` and `endTime`. The $i$-th meeting begins at `startTime[i]` and concludes at `endTime[i]`, inclusive.

The office manager wants to know how many meetings were active during a specific maintenance window `[queryStart, queryEnd]`. A meeting is considered active if their duration overlaps with the maintenance window at any point (even for a single moment).

Your task is to return the total number of meetings who were active during the given maintenance window.

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
The maintenance window is `[2, 4]`.
- Meeting 1 `[1, 3]` overlaps with `[2, 4]` (times 2, 3).
- Meeting 2 `[2, 2]` overlaps with `[2, 4]` (time 2).
- Meeting 3 `[3, 7]` overlaps with `[2, 4]` (times 3, 4).
All 3 meetings were active.

### 2

#### Input
1
4
4
1 3

#### Output
0

#### Explanation
The meeting was active at time `[4, 4]`. The maintenance window is `[1, 3]`. There is no overlap.

## Input Format
- The first line contains an integer `n`, the number of meetings.
- The second line contains `n` space-separated integers for `startTime`.
- The third line contains `n` space-separated integers for `endTime`.
- The fourth line contains two integers, `queryStart` and `queryEnd`.

## Output Format
- Return a single integer representing the number of meetings active during the maintenance window.

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
