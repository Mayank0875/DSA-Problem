## Title
Network Packet Routing

## Slug
network-packet-routing

## Difficulty
Medium

## Description
Data packets are scheduled for transmission. Each packet reserves a time window on the channel.

The queue has list of packets, each defined by a start time and an end time, represented as a pair `[start, end]`.

To avoid collision, the transmission end time of a packet must be strictly less than the start time of the subsequent packet. Specifically, to transition from packet `[a, b]` to a subsequent packet `[c, d]`, the end of the first packet must be **strictly less than** the start of the second packet (i.e., `b < c`).

You can select packets in any order you like to form a valid transmission stream. Your goal is to determine the maximum number of packets that can be included in a single transmission stream.

## Examples

### 1

#### Input
3
1 2
2 3
3 4

#### Output
2

#### Explanation
The longest transmission stream is `[1, 2] -> [3, 4]`. You cannot include `[2, 3]` because `2` (end of first) is not strictly less than `2` (start of second).

### 2

#### Input
3
1 2
7 8
4 5

#### Output
3

#### Explanation
The packets can be reordered to form the transmission stream `[1, 2] -> [4, 5] -> [7, 8]`. All transitions satisfy `end < start`.

## Input Format
- The first line contains an integer `n`, the number of available packets.
- The next `n` lines each contain two integers, representing the `start` and `end` of an packet.

## Output Format
- Return a single integer representing the maximum length of the transmission stream.

## Constraints
- 1 ≤ n ≤ 1000
- -1000 ≤ start < end ≤ 1000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy, sorting
