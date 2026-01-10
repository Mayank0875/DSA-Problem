## Title
Traffic Light Green Phase

## Slug
traffic-light-green-phase

## Difficulty
Easy

## Description
A city monitors how long cars wait at a light.

The traffic cam records the arrival and departure of every car in two integer arrays, `startTime` and `endTime`. The $i$-th car arrives at the line at `startTime[i]` and crosses the intersection at `endTime[i]`, inclusive.

The traffic engineer wants to know how many cars were waiting during a specific red light cycle `[queryStart, queryEnd]`. A car is considered waiting if their wait time overlaps with the red light cycle at any point (even for a single moment).

Your task is to return the total number of cars who were waiting during the given red light cycle.

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
The red light cycle is `[2, 4]`.
- Car 1 `[1, 3]` overlaps with `[2, 4]` (times 2, 3).
- Car 2 `[2, 2]` overlaps with `[2, 4]` (time 2).
- Car 3 `[3, 7]` overlaps with `[2, 4]` (times 3, 4).
All 3 cars were waiting.

### 2

#### Input
1
4
4
1 3

#### Output
0

#### Explanation
The car was waiting at time `[4, 4]`. The red light cycle is `[1, 3]`. There is no overlap.

## Input Format
- The first line contains an integer `n`, the number of cars.
- The second line contains `n` space-separated integers for `startTime`.
- The third line contains `n` space-separated integers for `endTime`.
- The fourth line contains two integers, `queryStart` and `queryEnd`.

## Output Format
- Return a single integer representing the number of cars waiting during the red light cycle.

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
