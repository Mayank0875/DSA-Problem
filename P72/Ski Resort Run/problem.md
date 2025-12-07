## Title
Ski Resort Run

## Slug
ski-resort-run

## Difficulty
Hard

## Description
A skier tackles the mountain. Starting at the Peak (1), they must reach the Lodge (n). Slopes connect various checkpoints.

The skier must start at the Peak (labeled 1) and finish at the Lodge (labeled n). However, to hit every checkpoint for the competition, the skier must visit **every single checkpoint exactly once** during the journey.

You are given the map of the checkpoints and the directed slopes connecting them. Your task is to calculate the total number of distinct valid paths the skier can take to complete the run. As the number of paths can be very large, print the answer modulo 1000000007.

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
- The first line contains two integers n and m: the number of checkpoints and the number of slopes.
- The checkpoints are numbered 1, 2, ..., n.
- The next m lines describe the slopes. Each line has two integers a and b, indicating a one-way slope from checkpoint a to checkpoint b.

## Output Format
- Return one integer: the number of possible run paths modulo 10^9+7.

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
