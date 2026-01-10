## Title
Zoom Meeting Participants

## Slug
zoom-meeting-participants

## Difficulty
Easy

## Description
A video conferencing tool logs participant connection times.

The meeting report records the join time and leave time of every participant in two integer arrays, `startTime` and `endTime`. The $i$-th participant joins at `startTime[i]` and leaves at `endTime[i]`, inclusive.

The host wants to know how many participants were connected during a specific presentation slot `[queryStart, queryEnd]`. A participant is considered connected if their connection overlaps with the presentation slot at any point (even for a single moment).

Your task is to return the total number of participants who were connected during the given presentation slot.

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
The presentation slot is `[2, 4]`.
- Participant 1 `[1, 3]` overlaps with `[2, 4]` (times 2, 3).
- Participant 2 `[2, 2]` overlaps with `[2, 4]` (time 2).
- Participant 3 `[3, 7]` overlaps with `[2, 4]` (times 3, 4).
All 3 participants were connected.

### 2

#### Input
1
4
4
1 3

#### Output
0

#### Explanation
The participant was connected at time `[4, 4]`. The presentation slot is `[1, 3]`. There is no overlap.

## Input Format
- The first line contains an integer `n`, the number of participants.
- The second line contains `n` space-separated integers for `startTime`.
- The third line contains `n` space-separated integers for `endTime`.
- The fourth line contains two integers, `queryStart` and `queryEnd`.

## Output Format
- Return a single integer representing the number of participants connected during the presentation slot.

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
