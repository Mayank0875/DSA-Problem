## Title
Power Grid Inspection

## Slug
power-grid-inspection

## Difficulty
Hard

## Description
An engineer inspects the grid. Starting at the Plant (1), they must reach the Main Substation (n). Substations are connected by power lines.

The engineer must start at the Plant (labeled 1) and finish at the Main Substation (labeled n). However, to check the transformers at every substation, the engineer must visit **every single substation exactly once** during the journey.

You are given the map of the substations and the directed power lines connecting them. Your task is to calculate the total number of distinct valid paths the engineer can take to complete the inspection. As the number of paths can be very large, print the answer modulo 1000000007.

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
There are two possible paths that visit every substation exactly once:
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
- The first line contains two integers n and m: the number of substations and the number of power lines.
- The substations are numbered 1, 2, ..., n.
- The next m lines describe the power lines. Each line has two integers a and b, indicating a one-way power line from substation a to substation b.

## Output Format
- Return one integer: the number of possible inspection paths modulo 10^9+7.

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
