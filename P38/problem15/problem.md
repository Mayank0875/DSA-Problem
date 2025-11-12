## Title

Previous Lower Data Value

## Slug

previous-lower-data-value

## Difficulty

Easy

## Description

You are navigating through a **Data Rift**, a stream of sequential data packets transmitted over time. For each packet, you need to determine the value of the nearest previous packet whose data size is **strictly lower** than the current packet's size. If no such earlier packet exists (either because it's the first packet or all prior packets have sizes greater than or equal to the current one), you should indicate this with `-1`. This information helps in identifying recent drops in data volume within the rift. Compute this value for every packet given the sequence of data sizes.

## Examples

### 1

#### Input

8
[100, 80, 60, 70, 60, 75, 85, 110]

#### Output

[-1, -1, -1, 60, -1, 60, 75, 85]

#### Explanation

Packet 0 (100): No previous packet, output -1.  
Packet 1 (80): Size 100 on packet 0 is not lower, output -1.  
Packet 2 (60): Sizes 100, 80 are not lower, output -1.  
Packet 3 (70): Size 60 on packet 2 is lower, output 60.  
Packet 4 (60): Sizes 100, 80, 60, 70. None are strictly lower, output -1.  
Packet 5 (75): Size 60 on packet 4 is the nearest lower, output 60.  
Packet 6 (85): Size 75 on packet 5 is the nearest lower, output 75.  
Packet 7 (110): Size 85 on packet 6 is the nearest lower, output 85.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All packet sizes are equal, so no strictly lower previous size exists for any packet.

## Input Format

The first line contains a single integer n, the number of packets.  
The second line contains n space-separated integers p_0, p_1, ..., p_[n-1], representing the data size of each packet.

## Output Format

Return array of integers. The i-th integer should be the data size of the nearest packet j < i such that p_j < p_i. If no such packet exists, then -1.

## Constraints

1 ≤ n ≤ 10^5  
1 ≤ p_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array