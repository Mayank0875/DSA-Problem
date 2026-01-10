## Title
Taxi Ride Duration

## Slug
taxi-ride-duration

## Difficulty
Easy

## Description
A taxi company tracks ride times.

The trip log records the pickup and dropoff of every ride in two integer arrays, `startTime` and `endTime`. The $i$-th ride begins at `startTime[i]` and ends at `endTime[i]`, inclusive.

The dispatcher wants to know how many rides were in progress during a specific traffic surge `[queryStart, queryEnd]`. A ride is considered in progress if their trip overlaps with the traffic surge at any point (even for a single moment).

Your task is to return the total number of rides who were in progress during the given traffic surge.

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
The traffic surge is `[2, 4]`.
- Ride 1 `[1, 3]` overlaps with `[2, 4]` (times 2, 3).
- Ride 2 `[2, 2]` overlaps with `[2, 4]` (time 2).
- Ride 3 `[3, 7]` overlaps with `[2, 4]` (times 3, 4).
All 3 rides were in progress.

### 2

#### Input
1
4
4
1 3

#### Output
0

#### Explanation
The ride was in progress at time `[4, 4]`. The traffic surge is `[1, 3]`. There is no overlap.

## Input Format
- The first line contains an integer `n`, the number of rides.
- The second line contains `n` space-separated integers for `startTime`.
- The third line contains `n` space-separated integers for `endTime`.
- The fourth line contains two integers, `queryStart` and `queryEnd`.

## Output Format
- Return a single integer representing the number of rides in progress during the traffic surge.

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
