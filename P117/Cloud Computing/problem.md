## Title
Cloud Computing

## Slug
cloud-computing

## Difficulty
Medium

## Description
Server racks are allocated. Enterprise clients get the fastest, Business (you) get the mid-tier, and Personal users get the shared connection.

There are $3n$ servers of varying speed available. The distribution follows a strict protocol. In each round, you must select any 3 servers. The parties then claim them based on the following rules:

1. The **Enterprise** takes the server with the **maximum** speed from the triplet.
2. You, the **Business**, take the server with the **second maximum** speed.
3. The **Personal** takes the remaining server (the one with the minimum speed).

This process repeats until all servers are distributed. Your goal as the Business is to maximize the total speed of the servers you acquire.

Given an array of integers `servers`, where `servers[i]` represents the speed of the $i$-th server, return the maximum total speed you can obtain.

## Examples

### 1

#### Input
6
2 4 1 2 7 8

#### Output
9

#### Explanation
You have 6 servers. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. Enterprise takes `8`, you take `7`, Personal takes `2`.
2. Pick the remaining `(1, 2, 4)`. Enterprise takes `4`, you take `2`, Personal takes `1`.
Total speed = $7 + 2 = 9$.

### 2

#### Input
3
2 4 5

#### Output
4

#### Explanation
There is only one triplet `(2, 4, 5)`. Enterprise takes `5`, you take `4`, Personal takes `2`. Total = 4.

## Input Format
- The first line contains a single integer $3n$, the number of servers.
- The second line contains $3n$ space-separated integers representing the `servers` array.

## Output Format
- Return a single integer representing the maximum total speed you can collect.

## Constraints
- 1 ≤ servers.length ≤ 10^5
- `servers.length` is divisible by 3.
- 1 ≤ servers[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sorting, greedy, math
