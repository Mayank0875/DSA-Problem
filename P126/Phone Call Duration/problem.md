## Title
Phone Call Duration

## Slug
phone-call-duration

## Difficulty
Easy

## Description
A telecom provider logs active calls.

The switchboard records the connect time and disconnect time of every call in two integer arrays, `startTime` and `endTime`. The $i$-th call connects at `startTime[i]` and disconnects at `endTime[i]`, inclusive.

The analyst wants to know how many calls were active during a specific network outage `[queryStart, queryEnd]`. A call is considered active if their duration overlaps with the network outage at any point (even for a single moment).

Your task is to return the total number of calls who were active during the given network outage.

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
The network outage is `[2, 4]`.
- Call 1 `[1, 3]` overlaps with `[2, 4]` (times 2, 3).
- Call 2 `[2, 2]` overlaps with `[2, 4]` (time 2).
- Call 3 `[3, 7]` overlaps with `[2, 4]` (times 3, 4).
All 3 calls were active.

### 2

#### Input
1
4
4
1 3

#### Output
0

#### Explanation
The call was active at time `[4, 4]`. The network outage is `[1, 3]`. There is no overlap.

## Input Format
- The first line contains an integer `n`, the number of calls.
- The second line contains `n` space-separated integers for `startTime`.
- The third line contains `n` space-separated integers for `endTime`.
- The fourth line contains two integers, `queryStart` and `queryEnd`.

## Output Format
- Return a single integer representing the number of calls active during the network outage.

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
