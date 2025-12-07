## Title
Spy Network Infiltration

## Slug
spy-network-infiltration

## Difficulty
Hard

## Description
An agent must deliver a message through a network of safehouses. Starting at Safehouse 1, the agent must reach Safehouse n using secure, one-way communication channels.

The agent must start at the Drop Point Alpha (labeled 1) and finish at the Extraction Point (labeled n). However, to verify the security status of every location manually, the agent must visit **every single safehouse exactly once** during the journey.

You are given the map of the safehouses and the directed channels connecting them. Your task is to calculate the total number of distinct valid paths the agent can take to complete the infiltration. As the number of paths can be very large, print the answer modulo 1000000007.

## Examples

### 1

#### Input
4 6
1 2
1 3
2 3
3 2
2 4
3 4

#### Output
2

#### Explanation
There are two possible paths that visit every safehouse exactly once:
1 -> 2 -> 3 -> 4
1 -> 3 -> 2 -> 4

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
The only valid path is 1 -> 2.

## Input Format
- The first line contains two integers n and m: the number of safehouses and the number of channels.
- The safehouses are numbered 1, 2, ..., n.
- The next m lines describe the channels. Each line has two integers a and b, indicating a one-way channel from safehouse a to safehouse b.

## Output Format
- Return one integer: the number of possible infiltration paths modulo 10^9+7.

## Constraints
- 1 ≤ n ≤ 20
- 1 ≤ m ≤ n * n
- 1 ≤ a, b ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, dynamic-programming
