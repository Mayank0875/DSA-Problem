## Title
Server Port Scan

## Slug
server-port-scan

## Difficulty
Medium

## Description
A firewall logs open ports. A hacker usually scans a range. The admin identifies the attack by finding the longest sequence of consecutive open ports.

Given an unsorted array of integers `ports` representing the port numbers, return the length of the longest consecutive sequence of ports that can be flagged as a scan attack.

You must write an algorithm that runs in $O(n)$ time.

## Examples

### 1

#### Input
6
100 4 200 1 3 2

#### Output
4

#### Explanation
The longest consecutive sequence is `[1, 2, 3, 4]`. Therefore its length is 4.

### 2

#### Input
10
0 3 7 2 5 8 4 6 0 1

#### Output
9

#### Explanation
The consecutive sequence is `[0, 1, 2, 3, 4, 5, 6, 7, 8]`. Note that duplicates are handled (ignored or treated as part of the set existence).

## Input Format
- The first line contains an integer `n`, the number of ports.
- The second line contains `n` space-separated integers representing the `ports` array.

## Output Format
- Return a single integer representing the length of the longest consecutive sequence.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ ports[i] ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table
