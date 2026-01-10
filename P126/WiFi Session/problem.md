## Title
WiFi Session

## Slug
wifi-session

## Difficulty
Easy

## Description
A public hotspot tracks user connections.

The router log records the connect time and disconnect time of every device in two integer arrays, `startTime` and `endTime`. The $i$-th device connects at `startTime[i]` and disconnects at `endTime[i]`, inclusive.

The network admin wants to know how many devices were connected during a specific bandwidth throttle `[queryStart, queryEnd]`. A device is considered connected if their session overlaps with the bandwidth throttle at any point (even for a single moment).

Your task is to return the total number of devices who were connected during the given bandwidth throttle.

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
The bandwidth throttle is `[2, 4]`.
- Device 1 `[1, 3]` overlaps with `[2, 4]` (times 2, 3).
- Device 2 `[2, 2]` overlaps with `[2, 4]` (time 2).
- Device 3 `[3, 7]` overlaps with `[2, 4]` (times 3, 4).
All 3 devices were connected.

### 2

#### Input
1
4
4
1 3

#### Output
0

#### Explanation
The device was connected at time `[4, 4]`. The bandwidth throttle is `[1, 3]`. There is no overlap.

## Input Format
- The first line contains an integer `n`, the number of devices.
- The second line contains `n` space-separated integers for `startTime`.
- The third line contains `n` space-separated integers for `endTime`.
- The fourth line contains two integers, `queryStart` and `queryEnd`.

## Output Format
- Return a single integer representing the number of devices connected during the bandwidth throttle.

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
