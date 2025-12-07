## Title
Drone Surveillance

## Slug
drone-surveillance

## Difficulty
Hard

## Description
A drone patrols a secure facility. Starting at the Charging Pad (1), it must reach the Hangar (n). Surveillance zones are connected by flight corridors.

The drone must start at the Charging Pad (labeled 1) and finish at the Hangar (labeled n). However, to scan every zone for intruders, the drone must visit **every single zone exactly once** during the journey.

You are given the map of the zones and the directed corridors connecting them. Your task is to calculate the total number of distinct valid paths the drone can take to complete the patrol. As the number of paths can be very large, print the answer modulo 1000000007.

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
There are two possible paths that visit every zone exactly once:
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
- The first line contains two integers n and m: the number of zones and the number of corridors.
- The zones are numbered 1, 2, ..., n.
- The next m lines describe the corridors. Each line has two integers a and b, indicating a one-way corridor from zone a to zone b.

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
