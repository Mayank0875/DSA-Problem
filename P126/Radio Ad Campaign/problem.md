## Title
Radio Ad Campaign

## Slug
radio-ad-campaign

## Difficulty
Easy

## Description
A station logs when ads are played.

The broadcast log records the start second and end second of every ad in two integer arrays, `startTime` and `endTime`. The $i$-th ad starts playing at `startTime[i]` and ends playing at `endTime[i]`, inclusive.

The producer wants to know how many ads were on air during a specific drive time block `[queryStart, queryEnd]`. A ad is considered on air if their airtime overlaps with the drive time block at any point (even for a single moment).

Your task is to return the total number of ads who were on air during the given drive time block.

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
The drive time block is `[2, 4]`.
- Ad 1 `[1, 3]` overlaps with `[2, 4]` (times 2, 3).
- Ad 2 `[2, 2]` overlaps with `[2, 4]` (time 2).
- Ad 3 `[3, 7]` overlaps with `[2, 4]` (times 3, 4).
All 3 ads were on air.

### 2

#### Input
1
4
4
1 3

#### Output
0

#### Explanation
The ad was on air at time `[4, 4]`. The drive time block is `[1, 3]`. There is no overlap.

## Input Format
- The first line contains an integer `n`, the number of ads.
- The second line contains `n` space-separated integers for `startTime`.
- The third line contains `n` space-separated integers for `endTime`.
- The fourth line contains two integers, `queryStart` and `queryEnd`.

## Output Format
- Return a single integer representing the number of ads on air during the drive time block.

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
