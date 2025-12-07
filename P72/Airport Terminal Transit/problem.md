## Title
Airport Terminal Transit

## Slug
airport-terminal-transit

## Difficulty
Hard

## Description
A passenger rushes for a connection. Starting at Gate 1, they must reach Gate n. Terminals are connected by walkways.

The passenger must start at the Gate 1 (labeled 1) and finish at the Gate n (labeled n). However, to stamp their passport at every section checkpoint, the passenger must visit **every single terminal section exactly once** during the journey.

You are given the map of the terminal sections and the directed walkways connecting them. Your task is to calculate the total number of distinct valid paths the passenger can take to complete the transit. As the number of paths can be very large, print the answer modulo 1000000007.

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
There are two possible paths that visit every terminal section exactly once:
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
- The first line contains two integers n and m: the number of terminal sections and the number of walkways.
- The terminal sections are numbered 1, 2, ..., n.
- The next m lines describe the walkways. Each line has two integers a and b, indicating a one-way walkway from terminal section a to terminal section b.

## Output Format
- Return one integer: the number of possible transit paths modulo 10^9+7.

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
