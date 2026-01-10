## Title
Bus Route Timing

## Slug
bus-route-timing

## Difficulty
Easy

## Description
A transit authority tracks buses on a route.

The GPS tracker records the route start and route end of every bus in two integer arrays, `startTime` and `endTime`. The $i$-th bus begins the route at `startTime[i]` and finishes the route at `endTime[i]`, inclusive.

The dispatcher wants to know how many buses were in service during a specific traffic jam `[queryStart, queryEnd]`. A bus is considered in service if their trip overlaps with the traffic jam at any point (even for a single moment).

Your task is to return the total number of buses who were in service during the given traffic jam.

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
The traffic jam is `[2, 4]`.
- Bus 1 `[1, 3]` overlaps with `[2, 4]` (times 2, 3).
- Bus 2 `[2, 2]` overlaps with `[2, 4]` (time 2).
- Bus 3 `[3, 7]` overlaps with `[2, 4]` (times 3, 4).
All 3 buses were in service.

### 2

#### Input
1
4
4
1 3

#### Output
0

#### Explanation
The bus was in service at time `[4, 4]`. The traffic jam is `[1, 3]`. There is no overlap.

## Input Format
- The first line contains an integer `n`, the number of buses.
- The second line contains `n` space-separated integers for `startTime`.
- The third line contains `n` space-separated integers for `endTime`.
- The fourth line contains two integers, `queryStart` and `queryEnd`.

## Output Format
- Return a single integer representing the number of buses in service during the traffic jam.

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
