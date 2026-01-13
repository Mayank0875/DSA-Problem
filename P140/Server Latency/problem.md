## Title
Server Latency

## Slug
server-latency

## Difficulty
Easy

## Description
A network admin checks ping times for various game servers.

The monitoring tool records the ping (ms) of $N$ servers in an array. To optimize routing, the admin needs to assign a rank to every server based on its ping (ms).

The ranking rules are simple: the server with the **smallest** ping (ms) gets **Rank 1**. The next distinct ping (ms) gets **Rank 2**, and so on.

If two or more servers have the exact same ping (ms), they must receive the **same rank**. The ranks must be integers starting from 1.

Your task is to replace each server's ping (ms) with its corresponding rank.

## Examples

### 1

#### Input
4
40 10 20 30

#### Output
4 1 2 3

#### Explanation
10 is the smallest (Rank 1). 20 is the second smallest (Rank 2). 30 is third (Rank 3). 40 is largest (Rank 4).

### 2

#### Input
3
2 2 2

#### Output
1 1 1

#### Explanation
All servers share the same ping (ms), so they share Rank 1.

## Input Format
- The first line contains an integer `n`, the number of servers.
- The second line contains `n` space-separated integers representing the ping (ms)s.

## Output Format
- Return an array of integers where each element is the rank of the corresponding server.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, sorting
