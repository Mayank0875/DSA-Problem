## Title
Network Packets

## Slug
network-packets

## Difficulty
Hard

## Description
Packets are aggregated into frames. The protocol of a frame is identified by the most common packet type ID.

The Router has a collection of $n$ packets, where each packet is represented by an integer ID.

To transmit data, The Router must partition these packets into several non-empty frames. Every packet from the original collection must belong to exactly one frame. From each frame, a "protocol ID" is extracted. The protocol ID is defined as the **mode** (most frequent element) of the packets in that frame. If a frame has multiple packets tied for the most frequent appearance, any one of them can be chosen as the protocol ID.

The Router collects all the extracted protocol IDs to form a final multiset. Your task is to calculate how many distinct final multisets can be created using this process. Two multisets are considered different if the frequency of any ID differs between them.

## Examples

### 1

#### Input
3
1 2 3

#### Output
7

#### Explanation
Any non-empty subset of {1, 2, 3} can be achieved, for a total of 7 multisets.

### 2

#### Input
3
1 2 2

#### Output
4

#### Explanation
We can generate 4 different multisets:
1. Partition into {1, 2, 2} -> protocol ID is 2 -> Result {2}.
2. Partition into {1, 2}, {2} -> protocol IDs 1, 2 or 2, 2 -> Result {1, 2} or {2, 2}. (Wait, if {1, 2} mode can be 1 or 2. If we pick 2, result is {2, 2}).
3. Partition into {1}, {2, 2} -> protocol IDs 1, 2 -> Result {1, 2}.
4. Partition into {1}, {2}, {2} -> protocol IDs 1, 2, 2 -> Result {1, 2, 2}.
Total distinct multisets: {2}, {2, 2}, {1, 2}, {1, 2, 2}.

## Input Format
- The first line contains an integer $n$, the number of packets.
- The second line contains $n$ space-separated integers representing the packet IDs.

## Output Format
- Return a single integer representing the number of different multisets of protocol IDs possible, modulo $998244353$.

## Constraints
- 1 ≤ n ≤ 5000
- 1 ≤ ID ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, math, combinatorics
