## Title
Satellite Visibility

## Slug
satellite-visibility

## Difficulty
Easy

## Description
An observatory tracks when satellites are visible overhead.

The tracking system records the rise time and set time of every satellite in two integer arrays, `startTime` and `endTime`. The $i$-th satellite becomes visible at `startTime[i]` and goes out of sight at `endTime[i]`, inclusive.

The astronomer wants to know how many satellites were visible during a specific observation window `[queryStart, queryEnd]`. A satellite is considered visible if their pass overlaps with the observation window at any point (even for a single moment).

Your task is to return the total number of satellites who were visible during the given observation window.

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
The observation window is `[2, 4]`.
- Satellite 1 `[1, 3]` overlaps with `[2, 4]` (times 2, 3).
- Satellite 2 `[2, 2]` overlaps with `[2, 4]` (time 2).
- Satellite 3 `[3, 7]` overlaps with `[2, 4]` (times 3, 4).
All 3 satellites were visible.

### 2

#### Input
1
4
4
1 3

#### Output
0

#### Explanation
The satellite was visible at time `[4, 4]`. The observation window is `[1, 3]`. There is no overlap.

## Input Format
- The first line contains an integer `n`, the number of satellites.
- The second line contains `n` space-separated integers for `startTime`.
- The third line contains `n` space-separated integers for `endTime`.
- The fourth line contains two integers, `queryStart` and `queryEnd`.

## Output Format
- Return a single integer representing the number of satellites visible during the observation window.

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
