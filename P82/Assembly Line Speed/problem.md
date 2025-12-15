## Title
Assembly Line Speed

## Slug
assembly-line-speed

## Difficulty
Easy

## Description
A factory has n machines. To prevent bottlenecks, each subsequent machine in a line should have strictly higher throughput.

You have throughput rates for n machines.
A smooth line consists of machines where throughput is strictly higher than the previous machine.

You must optimize the line to find the longest possible smooth line. You can skip any number of machines to form the sequence, but you must maintain the original placement order of the selected machines. Calculate the maximum number of machines that can form such a sequence.

## Examples

### 1

#### Input
8
7 3 5 3 6 2 9 8

#### Output
4

#### Explanation
The input contains: [7, 3, 5, 3, 6, 2, 9, 8]. The longest smooth lines (strictly increasing) include:
3, 5, 6, 9
3, 5, 6, 8
The length of these sequences is 4.

### 2

#### Input
5
5 4 3 2 1

#### Output
1

#### Explanation
Since the values are strictly decreasing, we can pick at most 1 machine.

## Input Format
- The first line contains an integer n: the number of machines.
- The second line contains n integers x_1, x_2 ... x_n: the throughput of each machine in order.

## Output Format
- Return one integer: the length of the longest valid smooth line.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, dynamic-programming, greedy
