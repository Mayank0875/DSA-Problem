## Title

Next Higher Data Packet in Data Rift

## Slug

next-higher-data-packet

## Difficulty

Easy

## Description

In the sprawling Data Rift, streams of data packets flow continuously. For each packet, engineers want to determine the size of the nearest future packet that is strictly larger. This insight helps them gauge data spikes and optimize routing strategies. If there is no future packet with a larger size (either because it is the last packet or all subsequent packets are smaller or equal), this should be indicated. Can you compute this for every packet in the stream?

## Examples

### 1

#### Input

8
[500, 400, 600, 300, 700, 450, 800, 500]

#### Output

[600, 600, 700, 700, 800, 800, -1, -1]

#### Explanation

Packet 0 (500): Next higher is 600 (Packet 2). Output 600.
Packet 1 (400): Next higher is 600 (Packet 2). Output 600.
Packet 2 (600): Next higher is 700 (Packet 4). Output 700.
Packet 3 (300): Next higher is 700 (Packet 4). Output 700.
Packet 4 (700): Next higher is 800 (Packet 6). Output 800.
Packet 5 (450): Next higher is 800 (Packet 6). Output 800.
Packet 6 (800): No future packet is higher. Output -1.
Packet 7 (500): No future packet exists. Output -1.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All packet sizes are equal, so no future packet has a higher size.

## Input Format

The first line contains a single integer n, the number of packets.
The second line contains n space-separated integers a_0, a_1, ..., a_[n-1], representing the size of each data packet.

## Output Format

Return array of integers. The i-th integer should be the size of the nearest packet j > i such that a_j > a_i. If no such packet exists, then -1.

## Constraints

1 ≤ n ≤ 10^5
1 ≤ a_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array