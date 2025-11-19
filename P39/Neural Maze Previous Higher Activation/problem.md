## Title

Neural Maze: Previous Higher Activation

## Slug

neural-maze-previous-higher-activation

## Difficulty

Easy

## Description

Imagine navigating a neural maze where each node has a certain activation level. As you arrive at each node, you look back (to the left) along the path you have taken and want to know the activation of the nearest node that has a strictly higher activation than the current one. If all previous nodes have lower or equal activation, or if it’s the first node, there is no such higher‑activation node to the left. Your goal is to determine this activation value for each position in the maze.

## Examples

### 1

#### Input

8
[30, 60, 90, 50, 80, 40, 70, 50]

#### Output

[-1, -1, -1, 90, 90, 80, 80, 70]

#### Explanation

Node 0 (30): No previous node. Output -1.
Node 1 (60): Node 0 (30) is lower. Output -1.
Node 2 (90): Nodes 0 (30), 1 (60) are lower. Output -1.
Node 3 (50): Node 2 (90) is the nearest higher. Output 90.
Node 4 (80): Node 2 (90) is the nearest higher. Output 90.
Node 5 (40): Node 4 (80) is the nearest higher. Output 80.
Node 6 (70): Node 4 (80) is the nearest higher. Output 80.
Node 7 (50): Node 6 (70) is the nearest higher. Output 70.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All nodes have equal activation, so no strictly higher previous node exists.

## Input Format

The first line contains a single integer n, the number of nodes.
The second line contains n space-separated integers h_0, h_1, ..., h_[n-1], representing the activation level of each node.

## Output Format

Return array of integers. The i-th integer should be the activation of the nearest node j < i such that h_j > h_i. If no such day exists, then -1.

## Constraints

1 ≤ n ≤ 10^5
1 ≤ h_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array