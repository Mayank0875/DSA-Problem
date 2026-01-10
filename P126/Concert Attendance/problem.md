## Title
Concert Attendance

## Slug
concert-attendance

## Difficulty
Easy

## Description
A venue tracks when attendees enter and leave a festival.

The turnstile data records the entry time and exit time of every attendee in two integer arrays, `startTime` and `endTime`. The $i$-th attendee enters at `startTime[i]` and leaves at `endTime[i]`, inclusive.

The event organizer wants to know how many attendees were in the venue during a specific headline act `[queryStart, queryEnd]`. A attendee is considered in the venue if their attendance overlaps with the headline act at any point (even for a single moment).

Your task is to return the total number of attendees who were in the venue during the given headline act.

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
The headline act is `[2, 4]`.
- Attendee 1 `[1, 3]` overlaps with `[2, 4]` (times 2, 3).
- Attendee 2 `[2, 2]` overlaps with `[2, 4]` (time 2).
- Attendee 3 `[3, 7]` overlaps with `[2, 4]` (times 3, 4).
All 3 attendees were in the venue.

### 2

#### Input
1
4
4
1 3

#### Output
0

#### Explanation
The attendee was in the venue at time `[4, 4]`. The headline act is `[1, 3]`. There is no overlap.

## Input Format
- The first line contains an integer `n`, the number of attendees.
- The second line contains `n` space-separated integers for `startTime`.
- The third line contains `n` space-separated integers for `endTime`.
- The fourth line contains two integers, `queryStart` and `queryEnd`.

## Output Format
- Return a single integer representing the number of attendees in the venue during the headline act.

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
