## Title

Synchronized Robots

## Slug

synchronized-robots

## Difficulty

Medium

## Description

A factory has N robots on an assembly line. Each robot `i` is programmed to perform its task every `A[i]` clock cycles. To improve efficiency, you want to synchronize them. You are allowed to reprogram exactly one robot, changing its cycle length to any integer between 1 and 10⁹ (inclusive). Your goal is to find the maximum possible "synchronization factor" (the greatest common divisor) of all N robot cycle lengths after this one change.

## Examples

### 1

#### Input

3 
[7, 6, 8]

#### Output

2

#### Explanation

If we reprogram the first robot (with 7 cycles) to have 4 cycles, the array becomes [4, 6, 8]. The greatest common divisor is 2, which is the maximum possible value.

### 2

#### Input

2
[100, 100]

#### Output

100

#### Explanation

We can "reprogram" a robot to its original cycle length (e.g., change 100 to 100).

## Input Format

- First line: integer 'n' representing the number of elements written on the blackboard .  
- Second line: 'n' integers representing the elements that are written on blackboard.
- You will be given the array as an input to your function

## Output Format

- Return an integer representing the greatest common divisor after making your move.

## Constraints

- 1 ≤ n ≤ 10^5
- 1 ≤ arr[i] ≤ 10^9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, prefix sum, suffix sum, math