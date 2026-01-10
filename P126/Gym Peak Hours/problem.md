## Title
Gym Peak Hours

## Slug
gym-peak-hours

## Difficulty
Easy

## Description
A fitness center logs member check-ins.

The access log records the check-in time and check-out time of every member in two integer arrays, `startTime` and `endTime`. The $i$-th member arrives at `startTime[i]` and departs at `endTime[i]`, inclusive.

The gym owner wants to know how many members were working out during a specific evening rush `[queryStart, queryEnd]`. A member is considered working out if their workout overlaps with the evening rush at any point (even for a single moment).

Your task is to return the total number of members who were working out during the given evening rush.

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
The evening rush is `[2, 4]`.
- Member 1 `[1, 3]` overlaps with `[2, 4]` (times 2, 3).
- Member 2 `[2, 2]` overlaps with `[2, 4]` (time 2).
- Member 3 `[3, 7]` overlaps with `[2, 4]` (times 3, 4).
All 3 members were working out.

### 2

#### Input
1
4
4
1 3

#### Output
0

#### Explanation
The member was working out at time `[4, 4]`. The evening rush is `[1, 3]`. There is no overlap.

## Input Format
- The first line contains an integer `n`, the number of members.
- The second line contains `n` space-separated integers for `startTime`.
- The third line contains `n` space-separated integers for `endTime`.
- The fourth line contains two integers, `queryStart` and `queryEnd`.

## Output Format
- Return a single integer representing the number of members working out during the evening rush.

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
