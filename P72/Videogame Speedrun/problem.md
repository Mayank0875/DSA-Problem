## Title
Videogame Speedrun

## Slug
videogame-speedrun

## Difficulty
Hard

## Description
A gamer plays a platformer. Starting at Level 1, they must reach the Credits (n). Levels are connected by warp pipes.

The gamer must start at the Level 1 (labeled 1) and finish at the Credits (labeled n). However, to collect the hidden gem in every level, the gamer must visit **every single level exactly once** during the journey.

You are given the map of the levels and the directed warp pipes connecting them. Your task is to calculate the total number of distinct valid paths the gamer can take to complete the speedrun. As the number of paths can be very large, print the answer modulo 1000000007.

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
There are two possible paths that visit every level exactly once:
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
- The first line contains two integers n and m: the number of levels and the number of warp pipes.
- The levels are numbered 1, 2, ..., n.
- The next m lines describe the warp pipes. Each line has two integers a and b, indicating a one-way warp pipe from level a to level b.

## Output Format
- Return one integer: the number of possible speedrun paths modulo 10^9+7.

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
