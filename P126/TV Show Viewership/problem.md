## Title
TV Show Viewership

## Slug
tv-show-viewership

## Difficulty
Easy

## Description
A streaming service tracks when users watch a specific channel.

The analytics engine records the tune-in time and tune-out time of every viewer in two integer arrays, `startTime` and `endTime`. The $i$-th viewer starts watching at `startTime[i]` and stops watching at `endTime[i]`, inclusive.

The advertiser wants to know how many viewers were watching during a specific ad slot `[queryStart, queryEnd]`. A viewer is considered watching if their viewing time overlaps with the ad slot at any point (even for a single moment).

Your task is to return the total number of viewers who were watching during the given ad slot.

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
The ad slot is `[2, 4]`.
- Viewer 1 `[1, 3]` overlaps with `[2, 4]` (times 2, 3).
- Viewer 2 `[2, 2]` overlaps with `[2, 4]` (time 2).
- Viewer 3 `[3, 7]` overlaps with `[2, 4]` (times 3, 4).
All 3 viewers were watching.

### 2

#### Input
1
4
4
1 3

#### Output
0

#### Explanation
The viewer was watching at time `[4, 4]`. The ad slot is `[1, 3]`. There is no overlap.

## Input Format
- The first line contains an integer `n`, the number of viewers.
- The second line contains `n` space-separated integers for `startTime`.
- The third line contains `n` space-separated integers for `endTime`.
- The fourth line contains two integers, `queryStart` and `queryEnd`.

## Output Format
- Return a single integer representing the number of viewers watching during the ad slot.

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
