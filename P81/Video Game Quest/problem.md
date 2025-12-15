## Title
Video Game Quest

## Slug
video-game-quest

## Difficulty
Medium

## Description
A player progresses from NPC 1 to NPC n.

The quest log has `n` NPCs and `m` directed tasks. Tasks may repeat between the same pair of NPCs and self-loops are allowed. A quest chain of length `k` is a sequence of exactly `k` directed tasks; NPCs and tasks may be visited multiple times.

Given `n`, `m`, `k` and a list of the `m` directed tasks (each task given as two integers `u` `v` meaning a directed task from `u` to `v`), compute the number of distinct quest chains that start at NPC 1 and end at NPC `n` with length exactly `k`. Output the answer modulo 1000000007.

## Examples

### 1

#### Input
3 4 8
1 2
2 3
3 1
3 2

#### Output
2

#### Explanation
We have 3 NPCs. We want the number of directed quest chains of length 8 from NPC 1 to NPC 3.
Valid length-8 quest chains:
1 -> 2 -> 3 -> 1 -> 2 -> 3 -> 1 -> 2 -> 3
1 -> 2 -> 3 -> 2 -> 3 -> 1 -> 2 -> 3
There are 2 such quest chains.

### 2

#### Input
3 4 2
1 2
2 3
3 1
3 2

#### Output
1

#### Explanation
Assuming the graph has tasks 1->2 and 2->3, the only quest chain of length 2 from NPC 1 to NPC 3 is:
1 -> 2 -> 3

## Input Format
- The first line contains three integers n, m, and k: the number of NPCs, tasks, and the required quest chain length.
- The next m lines describe the tasks. Each line contains two integers u and v, indicating a directed task from NPC u to NPC v.

## Output Format
- Return single integer: the number of quest chains modulo 10^9+7.

## Constraints
- 1 ≤ n ≤ 100
- 1 ≤ m ≤ 10^5
- 1 ≤ k ≤ 10^18
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, dynamic-programming
