## Title
Drone Flight Path

## Slug
drone-flight-path

## Difficulty
Easy

## Description
Air traffic control tracks drone flights in a zone.

The radar log records the takeoff and landing of every drone in two integer arrays, `startTime` and `endTime`. The $i$-th drone takes off at `startTime[i]` and lands at `endTime[i]`, inclusive.

The controller wants to know how many drones were airborne during a specific restricted window `[queryStart, queryEnd]`. A drone is considered airborne if their flight overlaps with the restricted window at any point (even for a single moment).

Your task is to return the total number of drones who were airborne during the given restricted window.

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
The restricted window is `[2, 4]`.
- Drone 1 `[1, 3]` overlaps with `[2, 4]` (times 2, 3).
- Drone 2 `[2, 2]` overlaps with `[2, 4]` (time 2).
- Drone 3 `[3, 7]` overlaps with `[2, 4]` (times 3, 4).
All 3 drones were airborne.

### 2

#### Input
1
4
4
1 3

#### Output
0

#### Explanation
The drone was airborne at time `[4, 4]`. The restricted window is `[1, 3]`. There is no overlap.

## Input Format
- The first line contains an integer `n`, the number of drones.
- The second line contains `n` space-separated integers for `startTime`.
- The third line contains `n` space-separated integers for `endTime`.
- The fourth line contains two integers, `queryStart` and `queryEnd`.

## Output Format
- Return a single integer representing the number of drones airborne during the restricted window.

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
