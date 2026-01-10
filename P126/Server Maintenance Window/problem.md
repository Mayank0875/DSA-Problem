## Title
Server Maintenance Window

## Slug
server-maintenance-window

## Difficulty
Easy

## Description
IT tracks server uptime and downtime windows.

The system log records the boot time and shutdown time of every server in two integer arrays, `startTime` and `endTime`. The $i$-th server boots up at `startTime[i]` and shuts down at `endTime[i]`, inclusive.

The sysadmin wants to know how many servers were online during a specific critical period `[queryStart, queryEnd]`. A server is considered online if their uptime overlaps with the critical period at any point (even for a single moment).

Your task is to return the total number of servers who were online during the given critical period.

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
The critical period is `[2, 4]`.
- Server 1 `[1, 3]` overlaps with `[2, 4]` (times 2, 3).
- Server 2 `[2, 2]` overlaps with `[2, 4]` (time 2).
- Server 3 `[3, 7]` overlaps with `[2, 4]` (times 3, 4).
All 3 servers were online.

### 2

#### Input
1
4
4
1 3

#### Output
0

#### Explanation
The server was online at time `[4, 4]`. The critical period is `[1, 3]`. There is no overlap.

## Input Format
- The first line contains an integer `n`, the number of servers.
- The second line contains `n` space-separated integers for `startTime`.
- The third line contains `n` space-separated integers for `endTime`.
- The fourth line contains two integers, `queryStart` and `queryEnd`.

## Output Format
- Return a single integer representing the number of servers online during the critical period.

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
