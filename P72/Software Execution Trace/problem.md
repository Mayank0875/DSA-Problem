## Title
Software Execution Trace

## Slug
software-execution-trace

## Difficulty
Hard

## Description
A debugger traces program flow. Starting at Main() (1), it must reach End() (n). Functions are connected by calls.

The execution must start at the Main() (labeled 1) and finish at the End() (labeled n). However, to verify the execution of every function block, the execution must visit **every single function exactly once** during the journey.

You are given the map of the functions and the directed calls connecting them. Your task is to calculate the total number of distinct valid paths the execution can take to complete the trace. As the number of paths can be very large, print the answer modulo 1000000007.

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
There are two possible paths that visit every function exactly once:
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
- The first line contains two integers n and m: the number of functions and the number of calls.
- The functions are numbered 1, 2, ..., n.
- The next m lines describe the calls. Each line has two integers a and b, indicating a one-way call from function a to function b.

## Output Format
- Return one integer: the number of possible trace paths modulo 10^9+7.

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
