## Title
Coral Reef Swim

## Slug
coral-reef-swim

## Difficulty
Hard

## Description
A diver explores a reef. Starting at the Anchor (1), they must reach the Cave (n). Coral heads are connected by currents.

The diver must start at the Anchor (labeled 1) and finish at the Cave (labeled n). However, to photograph every coral head, the diver must visit **every single coral head exactly once** during the journey.

You are given the map of the coral heads and the directed currents connecting them. Your task is to calculate the total number of distinct valid paths the diver can take to complete the dive. As the number of paths can be very large, print the answer modulo 1000000007.

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
There are two possible paths that visit every coral head exactly once:
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
- The first line contains two integers n and m: the number of coral heads and the number of currents.
- The coral heads are numbered 1, 2, ..., n.
- The next m lines describe the currents. Each line has two integers a and b, indicating a one-way current from coral head a to coral head b.

## Output Format
- Return one integer: the number of possible dive paths modulo 10^9+7.

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
