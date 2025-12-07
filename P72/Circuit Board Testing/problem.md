## Title
Circuit Board Testing

## Slug
circuit-board-testing

## Difficulty
Hard

## Description
A quality assurance robot tests a printed circuit board. It starts at Pin 1 and must end at Pin n. The pins are connected by directional traces.

The robot must start at the Input Pin (labeled 1) and finish at the Output Pin (labeled n). However, to check the conductivity of every pin, the robot must visit **every single pin exactly once** during the journey.

You are given the map of the pins and the directed traces connecting them. Your task is to calculate the total number of distinct valid paths the robot can take to complete the testing sequence. As the number of paths can be very large, print the answer modulo 1000000007.

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
There are two possible paths that visit every pin exactly once:
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
- The first line contains two integers n and m: the number of pins and the number of traces.
- The pins are numbered 1, 2, ..., n.
- The next m lines describe the traces. Each line has two integers a and b, indicating a one-way trace from pin a to pin b.

## Output Format
- Return one integer: the number of possible testing sequence paths modulo 10^9+7.

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
