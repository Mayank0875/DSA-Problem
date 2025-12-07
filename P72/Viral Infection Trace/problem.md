## Title
Viral Infection Trace

## Slug
viral-infection-trace

## Difficulty
Hard

## Description
A computer virus spreads from a Patient Zero computer (1) to a Mainframe (n). The computers are connected on a local network.

The virus must start at the Patient Zero (labeled 1) and finish at the Mainframe (labeled n). However, to infect every machine in the subnet before hitting the core, the virus must visit **every single computer exactly once** during the journey.

You are given the map of the computers and the directed connections connecting them. Your task is to calculate the total number of distinct valid paths the virus can take to complete the infection path. As the number of paths can be very large, print the answer modulo 1000000007.

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
There are two possible paths that visit every computer exactly once:
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
- The first line contains two integers n and m: the number of computers and the number of connections.
- The computers are numbered 1, 2, ..., n.
- The next m lines describe the connections. Each line has two integers a and b, indicating a one-way connection from computer a to computer b.

## Output Format
- Return one integer: the number of possible infection path paths modulo 10^9+7.

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
