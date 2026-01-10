## Title
Music Festival Set

## Slug
music-festival-set

## Difficulty
Easy

## Description
A festival tracks band performance times.

The stage schedule records the set start and set end of every band in two integer arrays, `startTime` and `endTime`. The $i$-th band starts playing at `startTime[i]` and finishes at `endTime[i]`, inclusive.

The sound engineer wants to know how many bands were on stage during a specific sunset slot `[queryStart, queryEnd]`. A band is considered on stage if their set overlaps with the sunset slot at any point (even for a single moment).

Your task is to return the total number of bands who were on stage during the given sunset slot.

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
The sunset slot is `[2, 4]`.
- Band 1 `[1, 3]` overlaps with `[2, 4]` (times 2, 3).
- Band 2 `[2, 2]` overlaps with `[2, 4]` (time 2).
- Band 3 `[3, 7]` overlaps with `[2, 4]` (times 3, 4).
All 3 bands were on stage.

### 2

#### Input
1
4
4
1 3

#### Output
0

#### Explanation
The band was on stage at time `[4, 4]`. The sunset slot is `[1, 3]`. There is no overlap.

## Input Format
- The first line contains an integer `n`, the number of bands.
- The second line contains `n` space-separated integers for `startTime`.
- The third line contains `n` space-separated integers for `endTime`.
- The fourth line contains two integers, `queryStart` and `queryEnd`.

## Output Format
- Return a single integer representing the number of bands on stage during the sunset slot.

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
