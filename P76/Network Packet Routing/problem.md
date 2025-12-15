## Title
Network Packet Routing

## Slug
network-packet-routing

## Difficulty
Hard

## Description
A router groups `n` packets into `k` transmission frames. Packets vary in size. The 'transmission delay' for a frame is calculated as the square of the total size of packets in that frame.

You must partition the sequence of packets into exactly `k` non-empty contiguous frames.
Each frame corresponds to a frame.
The "transmission delay" for a frame is calculated as the **square of the sum** of the sizes of the packets in that frame.

Your goal is to minimize the total transmission delay (the sum of the transmission delay values of all `k` frames).

## Examples

### 1

#### Input
8 3
2 3 1 2 2 3 4 1

#### Output
110

#### Explanation
We partition the packets into 3 frames: `[2, 3, 1]`, `[2, 2, 3]`, and `[4, 1]`.
The sums are 6, 7, 5.
The total transmission delay is $6^2 + 7^2 + 5^2 = 36 + 49 + 25 = 110$.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
225

#### Explanation
Only 1 frame is allowed, containing all packets. Sum = 15. transmission delay = $15^2 = 225$.

## Input Format
- The first line contains two integers `n` and `k`: the number of packets and the required number of frames.
- The second line contains `n` integers representing the sizes of each packet.

## Output Format
- Return one integer: the minimum total transmission delay.

## Constraints
- 1 ≤ k ≤ n ≤ 3000
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, array
