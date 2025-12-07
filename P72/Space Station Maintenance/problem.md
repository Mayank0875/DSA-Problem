## Title
Space Station Maintenance

## Slug
space-station-maintenance

## Difficulty
Hard

## Description
A drone inspects a space station. Starting at the Docking Bay (1), it must reach the Command Center (n). Modules are connected by airlocks.

The drone must start at the Docking Bay (labeled 1) and finish at the Command Center (labeled n). However, to verify the integrity of every module, the drone must visit **every single module exactly once** during the journey.

You are given the map of the modules and the directed airlocks connecting them. Your task is to calculate the total number of distinct valid paths the drone can take to complete the maintenance run. As the number of paths can be very large, print the answer modulo 1000000007.

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
There are two possible paths that visit every module exactly once:
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
- The first line contains two integers n and m: the number of modules and the number of airlocks.
- The modules are numbered 1, 2, ..., n.
- The next m lines describe the airlocks. Each line has two integers a and b, indicating a one-way airlock from module a to module b.

## Output Format
- Return one integer: the number of possible maintenance run paths modulo 10^9+7.

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
