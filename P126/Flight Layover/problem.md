## Title
Flight Layover

## Slug
flight-layover

## Difficulty
Easy

## Description
An airport tracks planes at gates.

The control tower records the arrival time and departure time of every plane in two integer arrays, `startTime` and `endTime`. The $i$-th plane arrives at `startTime[i]` and departs at `endTime[i]`, inclusive.

The ground controller wants to know how many planes were at the gate during a specific maintenance break `[queryStart, queryEnd]`. A plane is considered at the gate if their layover overlaps with the maintenance break at any point (even for a single moment).

Your task is to return the total number of planes who were at the gate during the given maintenance break.

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
The maintenance break is `[2, 4]`.
- Plane 1 `[1, 3]` overlaps with `[2, 4]` (times 2, 3).
- Plane 2 `[2, 2]` overlaps with `[2, 4]` (time 2).
- Plane 3 `[3, 7]` overlaps with `[2, 4]` (times 3, 4).
All 3 planes were at the gate.

### 2

#### Input
1
4
4
1 3

#### Output
0

#### Explanation
The plane was at the gate at time `[4, 4]`. The maintenance break is `[1, 3]`. There is no overlap.

## Input Format
- The first line contains an integer `n`, the number of planes.
- The second line contains `n` space-separated integers for `startTime`.
- The third line contains `n` space-separated integers for `endTime`.
- The fourth line contains two integers, `queryStart` and `queryEnd`.

## Output Format
- Return a single integer representing the number of planes at the gate during the maintenance break.

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
