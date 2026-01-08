## Title
Network Routing

## Slug
network-routing

## Difficulty
Hard

## Description
A packet travels through server nodes. It can hop to the adjacent node or use a fast lane to skip to the next.

The packet starts at node 0 and wishes to reach node $n$. On each move, The packet can hop forward either **1 node** or **2 nodes**.

Your task is to calculate the total number of distinct ways to reach exactly node $n$. Since the distance $n$ can be extremely large, return the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
2

#### Output
2

#### Explanation
There are two ways to reach node 2:
1. 1 node + 1 node
2. 2 nodes

### 2

#### Input
3

#### Output
3

#### Explanation
There are three ways:
1. 1 + 1 + 1
2. 1 + 2
3. 2 + 1

## Input Format
- The only input line has an integer $n$ — the target node.

## Output Format
- Return a single integer: the number of ways modulo $10^9 + 7$.

## Constraints
- 1 ≤ n ≤ 10^18

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, math

