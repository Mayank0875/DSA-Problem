## Title
Inferior Servers

## Slug
inferior-servers

## Difficulty
Medium

## Description
A data center manages server hardware.

You have a list of $n$ servers. Each server has two main properties: **uptime score** and **bandwidth**. You are given a 2D integer array `properties` where `properties[i] = [uptime score_i, bandwidth_i]` represents the attributes of the $i$-th server.

A server is considered **inferior** if there exists another server that has **both** strictly greater uptime score and strictly greater bandwidth.

More formally, the $i$-th server is inferior if there exists an index $j$ such that `uptime score_j > uptime score_i` and `bandwidth_j > bandwidth_i`.

Your task is to return the number of inferior servers.

## Examples

### 1

#### Input
3
5 5
6 3
3 6

#### Output
0

#### Explanation
No server has strictly greater uptime score and bandwidth than another.

### 2

#### Input
2
2 2
3 3

#### Output
1

#### Explanation
The first server (2, 2) is inferior because the second server (3, 3) has strictly greater uptime score and bandwidth.

## Input Format
- The first line contains an integer $n$, the number of servers.
- The next $n$ lines each contain two space-separated integers, representing the uptime score and bandwidth of a server.

## Output Format
- Return a single integer representing the number of inferior servers.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ uptime score, bandwidth ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy, sorting
