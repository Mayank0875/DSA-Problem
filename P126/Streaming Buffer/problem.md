## Title
Streaming Buffer

## Slug
streaming-buffer

## Difficulty
Easy

## Description
A video player logs buffering events.

The debug log records the buffer start and buffer end of every event in two integer arrays, `startTime` and `endTime`. The $i$-th event starts buffering at `startTime[i]` and resumes playback at `endTime[i]`, inclusive.

The developer wants to know how many events were buffering during a specific network drop `[queryStart, queryEnd]`. A event is considered buffering if their stall overlaps with the network drop at any point (even for a single moment).

Your task is to return the total number of events who were buffering during the given network drop.

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
The network drop is `[2, 4]`.
- Event 1 `[1, 3]` overlaps with `[2, 4]` (times 2, 3).
- Event 2 `[2, 2]` overlaps with `[2, 4]` (time 2).
- Event 3 `[3, 7]` overlaps with `[2, 4]` (times 3, 4).
All 3 events were buffering.

### 2

#### Input
1
4
4
1 3

#### Output
0

#### Explanation
The event was buffering at time `[4, 4]`. The network drop is `[1, 3]`. There is no overlap.

## Input Format
- The first line contains an integer `n`, the number of events.
- The second line contains `n` space-separated integers for `startTime`.
- The third line contains `n` space-separated integers for `endTime`.
- The fourth line contains two integers, `queryStart` and `queryEnd`.

## Output Format
- Return a single integer representing the number of events buffering during the network drop.

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
