## Title
Network Packet Routing

## Slug
network-packet-routing

## Difficulty
Medium

## Description
A router buffers incoming bytes. Bytes are grouped into frames before being sent over the wire.

The Network Admin is working with a sequence of $n$ bytes, where the $i$-th byte has a value of $a_i$.

The Network Admin needs to create a **framing strategy**. A framing strategy involves dividing the sequence of $n$ bytes into one or more contiguous frames such that every byte belongs to exactly one frame.

For a specific framing strategy, the **checksum** is calculated as follows:
1. Calculate the sum of values for each frame in the partition.
2. The checksum is the bitwise XOR sum of these frame sums.

Your task is to calculate the bitwise XOR sum of the checksum values of **all possible framing strategys** of the sequence.

## Examples

### 1

#### Input
1
1

#### Output
1

#### Explanation
Total XOR sum: 1.

### 2

#### Input
2
1 2

#### Output
0

#### Explanation
Partition {1}, {2}: Group sums are 1, 2. XOR sum = 1 ^ 2 = 3.
Partition {1, 2}: Group sum is 3. XOR sum = 3.
Total Result = 3 ^ 3 = 0.

## Input Format
- The first line contains a single integer $n$ — the length of the sequence.
- The second line contains $n$ space-separated integers $a_1, a_2, \dots, a_n$.

## Output Format
- Return a single integer representing the total XOR sum of checksums of all possible partitions.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming, array
