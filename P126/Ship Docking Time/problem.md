## Title
Ship Docking Time

## Slug
ship-docking-time

## Difficulty
Easy

## Description
A port authority manages dock schedules.

The harbor log records the docking time and undocking time of every ship in two integer arrays, `startTime` and `endTime`. The $i$-th ship docks at `startTime[i]` and undocks at `endTime[i]`, inclusive.

The harbormaster wants to know how many ships were at berth during a specific storm surge `[queryStart, queryEnd]`. A ship is considered at berth if their berthing overlaps with the storm surge at any point (even for a single moment).

Your task is to return the total number of ships who were at berth during the given storm surge.

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
The storm surge is `[2, 4]`.
- Ship 1 `[1, 3]` overlaps with `[2, 4]` (times 2, 3).
- Ship 2 `[2, 2]` overlaps with `[2, 4]` (time 2).
- Ship 3 `[3, 7]` overlaps with `[2, 4]` (times 3, 4).
All 3 ships were at berth.

### 2

#### Input
1
4
4
1 3

#### Output
0

#### Explanation
The ship was at berth at time `[4, 4]`. The storm surge is `[1, 3]`. There is no overlap.

## Input Format
- The first line contains an integer `n`, the number of ships.
- The second line contains `n` space-separated integers for `startTime`.
- The third line contains `n` space-separated integers for `endTime`.
- The fourth line contains two integers, `queryStart` and `queryEnd`.

## Output Format
- Return a single integer representing the number of ships at berth during the storm surge.

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
