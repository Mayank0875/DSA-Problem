## Title
Hotel Room Management

## Slug
hotel-room-management

## Difficulty
Medium

## Description
A hotel has n rooms. Management identifies floor managers responsible for blocks of k rooms.

The Manager defines the "Supervision Scope" of the structure rooted at a specific room `r` as follows:
Consider every possible set of `k` distinct rooms from the structure.
1. For each set, find the Lowest Common Ancestor (LCA) of the rooms in that set, calculated with respect to the root `r`.
2. Let `S_r` be the set of all unique rooms obtained as LCAs from these sets.
3. The Supervision Scope of the structure rooted at `r` is the size of `S_r` (denoted as `|S_r|`).

The total "Management Index" is defined as the sum of the Supervision Scope values for all possible roots `r` from 1 to `n`:
Management Index = sum over `r` from 1 to `n` of `|S_r|`

Your task is to calculate the Management Index of the given hotel map.

Notes:
1. A hotel map is a connected graph without cycles.
2. The LCA of a set of nodes in a rooted hotel map is the deepest node that is an ancestor of all nodes in the set.

## Examples

### 1

#### Input
6 3
1 2
1 3
2 4
2 5
3 6

#### Output
17

#### Explanation
The calculated Management Index is 17.

### 2

#### Input
2 2
1 2

#### Output
2

#### Explanation
The calculated Management Index is 2.

## Input Format
- The first line of each test case contains two integers `n` and `k` — the number of rooms and the size of the sets to consider.
- The following `n-1` lines describe the hotel map. Each line contains two integers `u` and `v`, indicating a connection between rooms `u` and `v`.

## Output Format
- Return one integer: the Management Index.

## Constraints
- 1 ≤ k ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
depth-first-search, graph
