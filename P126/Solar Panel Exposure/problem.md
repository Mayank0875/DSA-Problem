## Title
Solar Panel Exposure

## Slug
solar-panel-exposure

## Difficulty
Easy

## Description
A solar farm tracks when panels receive direct sunlight.

The sensor array records the exposure start and exposure end of every panel in two integer arrays, `startTime` and `endTime`. The $i$-th panel starts receiving light at `startTime[i]` and stops receiving light at `endTime[i]`, inclusive.

The engineer wants to know how many panels were generating power during a specific peak sun hour `[queryStart, queryEnd]`. A panel is considered generating power if their exposure overlaps with the peak sun hour at any point (even for a single moment).

Your task is to return the total number of panels who were generating power during the given peak sun hour.

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
The peak sun hour is `[2, 4]`.
- Panel 1 `[1, 3]` overlaps with `[2, 4]` (times 2, 3).
- Panel 2 `[2, 2]` overlaps with `[2, 4]` (time 2).
- Panel 3 `[3, 7]` overlaps with `[2, 4]` (times 3, 4).
All 3 panels were generating power.

### 2

#### Input
1
4
4
1 3

#### Output
0

#### Explanation
The panel was generating power at time `[4, 4]`. The peak sun hour is `[1, 3]`. There is no overlap.

## Input Format
- The first line contains an integer `n`, the number of panels.
- The second line contains `n` space-separated integers for `startTime`.
- The third line contains `n` space-separated integers for `endTime`.
- The fourth line contains two integers, `queryStart` and `queryEnd`.

## Output Format
- Return a single integer representing the number of panels generating power during the peak sun hour.

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
