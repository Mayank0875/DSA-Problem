## Title
Network Packet Traffic

## Slug
network-packet-traffic

## Difficulty
Easy

## Description
A router analyzes data packet transmission windows.

The firewall log records the start timestamp and end timestamp of every packet in two integer arrays, `startTime` and `endTime`. The $i$-th packet starts transmitting at `startTime[i]` and finishes transmitting at `endTime[i]`, inclusive.

The network admin wants to know how many packets were in transit during a specific congestion spike `[queryStart, queryEnd]`. A packet is considered in transit if their transmission overlaps with the congestion spike at any point (even for a single moment).

Your task is to return the total number of packets who were in transit during the given congestion spike.

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
The congestion spike is `[2, 4]`.
- Packet 1 `[1, 3]` overlaps with `[2, 4]` (times 2, 3).
- Packet 2 `[2, 2]` overlaps with `[2, 4]` (time 2).
- Packet 3 `[3, 7]` overlaps with `[2, 4]` (times 3, 4).
All 3 packets were in transit.

### 2

#### Input
1
4
4
1 3

#### Output
0

#### Explanation
The packet was in transit at time `[4, 4]`. The congestion spike is `[1, 3]`. There is no overlap.

## Input Format
- The first line contains an integer `n`, the number of packets.
- The second line contains `n` space-separated integers for `startTime`.
- The third line contains `n` space-separated integers for `endTime`.
- The fourth line contains two integers, `queryStart` and `queryEnd`.

## Output Format
- Return a single integer representing the number of packets in transit during the congestion spike.

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
