## Title
Network Latency Test

## Slug
network-latency-test

## Difficulty
Easy

## Description
An admin tests ping times to n servers. They want to identify a pattern of increasing lag.

You have ping times for n servers.
A lag spike pattern consists of servers where the ping is strictly higher than the previous one.

You must analyze logs to find the longest possible lag pattern. You can skip any number of pings to form the sequence, but you must maintain the original sequential order of the selected pings. Calculate the maximum number of pings that can form such a sequence.

## Examples

### 1

#### Input
8
7 3 5 3 6 2 9 8

#### Output
4

#### Explanation
The input contains: [7, 3, 5, 3, 6, 2, 9, 8]. The longest lag patterns (strictly increasing) include:
3, 5, 6, 9
3, 5, 6, 8
The length of these sequences is 4.

### 2

#### Input
5
5 4 3 2 1

#### Output
1

#### Explanation
Since the values are strictly decreasing, we can pick at most 1 ping.

## Input Format
- The first line contains an integer n: the number of pings.
- The second line contains n integers x_1, x_2 ... x_n: the time of each ping in order.

## Output Format
- Return one integer: the length of the longest valid lag pattern.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, dynamic-programming, greedy
