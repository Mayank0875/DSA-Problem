## Title
Charging Station Usage

## Slug
charging-station-usage

## Difficulty
Easy

## Description
An EV network tracks charging sessions.

The station log records the plug-in and unplug of every car in two integer arrays, `startTime` and `endTime`. The $i$-th car starts charging at `startTime[i]` and stops charging at `endTime[i]`, inclusive.

The grid operator wants to know how many cars were charging during a specific peak rate window `[queryStart, queryEnd]`. A car is considered charging if their charge overlaps with the peak rate window at any point (even for a single moment).

Your task is to return the total number of cars who were charging during the given peak rate window.

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
The peak rate window is `[2, 4]`.
- Car 1 `[1, 3]` overlaps with `[2, 4]` (times 2, 3).
- Car 2 `[2, 2]` overlaps with `[2, 4]` (time 2).
- Car 3 `[3, 7]` overlaps with `[2, 4]` (times 3, 4).
All 3 cars were charging.

### 2

#### Input
1
4
4
1 3

#### Output
0

#### Explanation
The car was charging at time `[4, 4]`. The peak rate window is `[1, 3]`. There is no overlap.

## Input Format
- The first line contains an integer `n`, the number of cars.
- The second line contains `n` space-separated integers for `startTime`.
- The third line contains `n` space-separated integers for `endTime`.
- The fourth line contains two integers, `queryStart` and `queryEnd`.

## Output Format
- Return a single integer representing the number of cars charging during the peak rate window.

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
