## Title
Submarine Patrol

## Slug
submarine-patrol

## Difficulty
Hard

## Description
A submarine patrols a sector of the ocean. It starts at Base Alpha (1) and docks at Base Omega (n). The checkpoints are connected by deep-sea currents.

The submarine must start at the Base Alpha (labeled 1) and finish at the Base Omega (labeled n). However, to scan every checkpoint for enemy activity, the submarine must visit **every single checkpoint exactly once** during the journey.

You are given the map of the checkpoints and the directed currents connecting them. Your task is to calculate the total number of distinct valid paths the submarine can take to complete the patrol. As the number of paths can be very large, print the answer modulo 1000000007.

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
There are two possible paths that visit every checkpoint exactly once:
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
- The first line contains two integers n and m: the number of checkpoints and the number of currents.
- The checkpoints are numbered 1, 2, ..., n.
- The next m lines describe the currents. Each line has two integers a and b, indicating a one-way current from checkpoint a to checkpoint b.

## Output Format
- Return one integer: the number of possible patrol paths modulo 10^9+7.

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
