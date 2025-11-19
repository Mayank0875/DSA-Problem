## Title

Next Higher Encryption Level in Encrypted Valley

## Slug

next-higher-encryption-level

## Difficulty

Easy

## Description

The inhabitants of Encrypted Valley are analyzing the security levels of their data nodes to plan future upgrades. For each node, they want to identify the security level of the nearest subsequent node that has a strictly higher encryption strength. This helps them understand security improvement trends or spot critical upgrade points. If no later node has a higher level (either because it is the last node or all subsequent nodes have lower or equal encryption), this should be noted. Can you calculate this for each node?

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
Node 6 (800): No future node is higher. Output -1.
Node 7 (500): No future node exists. Output -1.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All encryption levels are equal, so no future node has a higher level.

## Input Format

The first line contains a single integer n, the number of nodes.
The second line contains n space-separated integers a_0, a_1, ..., a_[n-1], representing the encryption level for each node.

## Output Format

Return array of integers. The i-th integer should be the encryption level of the nearest node j > i such that a_j > a_i. If no such node exists, then -1.

## Constraints

1 ≤ n ≤ 10^5
1 ≤ a_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array