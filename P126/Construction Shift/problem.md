## Title
Construction Shift

## Slug
construction-shift

## Difficulty
Easy

## Description
A foreman tracks worker shifts on a site.

The time clock records the clock-in time and clock-out time of every worker in two integer arrays, `startTime` and `endTime`. The $i$-th worker starts work at `startTime[i]` and ends work at `endTime[i]`, inclusive.

The foreman wants to know how many workers were on site during a specific inspection period `[queryStart, queryEnd]`. A worker is considered on site if their shift overlaps with the inspection period at any point (even for a single moment).

Your task is to return the total number of workers who were on site during the given inspection period.

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
The inspection period is `[2, 4]`.
- Worker 1 `[1, 3]` overlaps with `[2, 4]` (times 2, 3).
- Worker 2 `[2, 2]` overlaps with `[2, 4]` (time 2).
- Worker 3 `[3, 7]` overlaps with `[2, 4]` (times 3, 4).
All 3 workers were on site.

### 2

#### Input
1
4
4
1 3

#### Output
0

#### Explanation
The worker was on site at time `[4, 4]`. The inspection period is `[1, 3]`. There is no overlap.

## Input Format
- The first line contains an integer `n`, the number of workers.
- The second line contains `n` space-separated integers for `startTime`.
- The third line contains `n` space-separated integers for `endTime`.
- The fourth line contains two integers, `queryStart` and `queryEnd`.

## Output Format
- Return a single integer representing the number of workers on site during the inspection period.

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
