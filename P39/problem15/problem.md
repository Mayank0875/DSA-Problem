## Title

Previous Higher Data Packet in the Rift

## Slug

previous-higher-data-packet

## Difficulty

Easy

## Description

Imagine navigating through a data stream in a massive digital rift, where each data packet has a certain size. As you examine each packet, you look back (to earlier packets) and want to know the size of the nearest packet that is strictly larger than the current one. If all previous packets are smaller or of equal size, or if it's the first packet, there is no such larger packet to the left. Your goal is to determine this larger packet's size for each position in the stream.

## Examples

### 1

#### Input

8
[30, 60, 90, 50, 80, 40, 70, 50]

#### Output

[-1, -1, -1, 90, 90, 80, 80, 70]

#### Explanation

Packet 0 (30): No previous packet. Output -1.
Packet 1 (60): Packet 0 (30) is smaller. Output -1.
Packet 2 (90): Packets 0 (30), 1 (60) are smaller. Output -1.
Packet 3 (50): Packet 2 (90) is the nearest larger. Output 90.
Packet 4 (80): Packet 2 (90) is the nearest larger. Output 90.
Packet 5 (40): Packet 4 (80) is the nearest larger. Output 80.
Packet 6 (70): Packet 4 (80) is the nearest larger. Output 80.
Packet 7 (50): Packet 6 (70) is the nearest larger. Output 70.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All packets are equal, so no strictly larger previous packet exists.

## Input Format

The first line contains a single integer n, the number of packets.
The second line contains n space-separated integers h_0, h_1, ..., h_[n-1], representing the size of each packet.

## Output Format

Return array of integers. The i-th integer should be the size of the nearest packet j < i such that h_j > h_i. If no such day exists, then -1.

## Constraints

1 ≤ n ≤ 10^5
1 ≤ h_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array