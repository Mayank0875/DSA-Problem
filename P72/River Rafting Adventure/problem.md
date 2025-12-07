## Title
River Rafting Adventure

## Slug
river-rafting-adventure

## Difficulty
Hard

## Description
Rafters navigate a river system. Starting at the Put-in (1), they must reach the Take-out (n). The river has various docks connected by rapids.

The rafter must start at the Put-in (labeled 1) and finish at the Take-out (labeled n). However, to stamp their logbook at every dock, the rafter must visit **every single dock exactly once** during the journey.

You are given the map of the docks and the directed rapids connecting them. Your task is to calculate the total number of distinct valid paths the rafter can take to complete the adventure. As the number of paths can be very large, print the answer modulo 1000000007.

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
There are two possible paths that visit every dock exactly once:
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
- The first line contains two integers n and m: the number of docks and the number of rapids.
- The docks are numbered 1, 2, ..., n.
- The next m lines describe the rapids. Each line has two integers a and b, indicating a one-way rapid from dock a to dock b.

## Output Format
- Return one integer: the number of possible adventure paths modulo 10^9+7.

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
