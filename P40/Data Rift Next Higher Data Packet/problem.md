## Title

Data Rift: Next Higher Data Packet

## Slug

data-rift-next-higher-data-packet

## Difficulty

Easy

## Description

In the sprawling Data Rift, streams of data packets flow through a series of nodes. For each node, engineers need to determine the size of the nearest future packet that is strictly larger than the current one. This information helps in optimizing bandwidth allocation and detecting spikes in data flow. If no later packet has a larger size (either because it is the last node or all subsequent packets are smaller or equal), this should be indicated. Can you compute this for every node?

## Examples

### 1

#### Input

8
[500, 400, 600, 300, 700, 450, 800, 500]

#### Output

[600, 600, 700, 700, 800, 800, -1, -1]

#### Explanation

Node 0 (500): Next higher is 600 (Node 2). Output 600.
Node 1 (400): Next higher is 600 (Node 2). Output 600.
Node 2 (600): Next higher is 700 (Node 4). Output 700.
Node 3 (300): Next higher is 700 (Node 4). Output 700.
Node 4 (700): Next higher is 800 (Node 6). Output 800.
Node 5 (450): Next higher is 800 (Node 6). Output 800.
Node 6 (800): No future packet is higher. Output -1.
Node 7 (500): No future packet exists. Output -1.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All packet sizes are equal, so no future packet has a higher size.

## Input Format

The first line contains a single integer n, the number of nodes.
The second line contains n space-separated integers a_0, a_1, ..., a_[n-1], representing the size of the data packet at each node.

## Output Format

Return array of integers. The i-th integer should be the size of the nearest node j > i such that a_j > a_i. If no such node exists, then -1.

## Constraints

1 ≤ n ≤ 10^5
1 ≤ a_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array