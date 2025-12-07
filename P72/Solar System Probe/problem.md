## Title
Solar System Probe

## Slug
solar-system-probe

## Difficulty
Hard

## Description
A probe explores a solar system. Starting at the Sun (1), it must reach the Outer Belt (n). Planets are connected by gravity assists.

The probe must start at the Sun (labeled 1) and finish at the Outer Belt (labeled n). However, to collect data from every planet, the probe must visit **every single planet exactly once** during the journey.

You are given the map of the planets and the directed trajectories connecting them. Your task is to calculate the total number of distinct valid paths the probe can take to complete the mission. As the number of paths can be very large, print the answer modulo 1000000007.

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
There are two possible paths that visit every planet exactly once:
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
- The first line contains two integers n and m: the number of planets and the number of trajectories.
- The planets are numbered 1, 2, ..., n.
- The next m lines describe the trajectories. Each line has two integers a and b, indicating a one-way trajectory from planet a to planet b.

## Output Format
- Return one integer: the number of possible mission paths modulo 10^9+7.

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
