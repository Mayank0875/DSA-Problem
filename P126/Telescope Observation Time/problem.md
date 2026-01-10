## Title
Telescope Observation Time

## Slug
telescope-observation-time

## Difficulty
Easy

## Description
Researchers book time on a space telescope.

The schedule records the booking start and booking end of every researcher in two integer arrays, `startTime` and `endTime`. The $i$-th researcher begins observation at `startTime[i]` and ends observation at `endTime[i]`, inclusive.

The facility manager wants to know how many researchers were using the telescope during a specific satellite pass `[queryStart, queryEnd]`. A researcher is considered using the telescope if their slot overlaps with the satellite pass at any point (even for a single moment).

Your task is to return the total number of researchers who were using the telescope during the given satellite pass.

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
The satellite pass is `[2, 4]`.
- Researcher 1 `[1, 3]` overlaps with `[2, 4]` (times 2, 3).
- Researcher 2 `[2, 2]` overlaps with `[2, 4]` (time 2).
- Researcher 3 `[3, 7]` overlaps with `[2, 4]` (times 3, 4).
All 3 researchers were using the telescope.

### 2

#### Input
1
4
4
1 3

#### Output
0

#### Explanation
The researcher was using the telescope at time `[4, 4]`. The satellite pass is `[1, 3]`. There is no overlap.

## Input Format
- The first line contains an integer `n`, the number of researchers.
- The second line contains `n` space-separated integers for `startTime`.
- The third line contains `n` space-separated integers for `endTime`.
- The fourth line contains two integers, `queryStart` and `queryEnd`.

## Output Format
- Return a single integer representing the number of researchers using the telescope during the satellite pass.

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
