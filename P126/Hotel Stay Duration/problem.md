## Title
Hotel Stay Duration

## Slug
hotel-stay-duration

## Difficulty
Easy

## Description
A hotel tracks guest bookings.

The reservation system records the check-in date and check-out date of every guest in two integer arrays, `startTime` and `endTime`. The $i$-th guest checks in at `startTime[i]` and checks out at `endTime[i]`, inclusive.

The manager wants to know how many guests were staying during a specific holiday weekend `[queryStart, queryEnd]`. A guest is considered staying if their visit overlaps with the holiday weekend at any point (even for a single moment).

Your task is to return the total number of guests who were staying during the given holiday weekend.

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
The holiday weekend is `[2, 4]`.
- Guest 1 `[1, 3]` overlaps with `[2, 4]` (times 2, 3).
- Guest 2 `[2, 2]` overlaps with `[2, 4]` (time 2).
- Guest 3 `[3, 7]` overlaps with `[2, 4]` (times 3, 4).
All 3 guests were staying.

### 2

#### Input
1
4
4
1 3

#### Output
0

#### Explanation
The guest was staying at time `[4, 4]`. The holiday weekend is `[1, 3]`. There is no overlap.

## Input Format
- The first line contains an integer `n`, the number of guests.
- The second line contains `n` space-separated integers for `startTime`.
- The third line contains `n` space-separated integers for `endTime`.
- The fourth line contains two integers, `queryStart` and `queryEnd`.

## Output Format
- Return a single integer representing the number of guests staying during the holiday weekend.

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
