## Title
Robot Assembly Line

## Slug
robot-assembly-line

## Difficulty
Hard

## Description
A part moves through a factory. Starting at Intake (1), it must reach Packaging (n). Workstations are connected by conveyor belts.

The part must start at the Intake (labeled 1) and finish at the Packaging (labeled n). However, to undergo processing at every station, the part must visit **every single workstation exactly once** during the journey.

You are given the map of the workstations and the directed belts connecting them. Your task is to calculate the total number of distinct valid paths the part can take to complete the assembly. As the number of paths can be very large, print the answer modulo 1000000007.

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
There are two possible paths that visit every workstation exactly once:
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
- The first line contains two integers n and m: the number of workstations and the number of belts.
- The workstations are numbered 1, 2, ..., n.
- The next m lines describe the belts. Each line has two integers a and b, indicating a one-way belt from workstation a to workstation b.

## Output Format
- Return one integer: the number of possible assembly paths modulo 10^9+7.

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
