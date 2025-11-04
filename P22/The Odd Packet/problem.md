## Title

The Odd Packet

## Slug

the-odd-packet

## Difficulty

Medium

## Description

A data stream consists of packets, sorted by their sequence number. The protocol requires that every packet is sent twice for verification. The stream is guaranteed to have every packet twice in a row, except for one packet that was dropped and appears only once. Find the sequence number of this single, unduplicated packet.

You must write an algorithm with O(log n) runtime complexity.

## Examples

### 1

#### Input

9 
[1, 1, 2, 3, 3, 4, 4, 8, 8]


#### Output

2

#### Explanation

In the sequence [1, 1, 2, 3, 3, 4, 4, 8, 8], the number 2 appears only once.

### 2

#### Input

7 
[3, 3, 7, 7, 10, 11, 11]

#### Output

10

#### Explanation

In the sequence [3, 3, 7, 7, 10, 11, 11], the number 10 appears only once.

## Input Format

- The first line contains an odd integer n, the total number of packets.
- The second line contains n space-separated integers representing the sorted sequence numbers.

## Output Format

- Return a single integer: the sequence number of the packet that appears only once.

## Constraints

- 1 ≤ n ≤ 10^5
- 1 ≤ stone_value ≤ 10^9
- The array is sorted.
- Every element appears twice except for one.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, array