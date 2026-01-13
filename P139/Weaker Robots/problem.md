## Title
Weaker Robots

## Slug
weaker-robots

## Difficulty
Medium

## Description
A robotics lab tests prototypes.

You have a list of $n$ robots. Each robot has two main properties: **battery life** and **torque**. You are given a 2D integer array `properties` where `properties[i] = [battery life_i, torque_i]` represents the attributes of the $i$-th robot.

A robot is considered **weaker** if there exists another robot that has **both** strictly greater battery life and strictly greater torque.

More formally, the $i$-th robot is weaker if there exists an index $j$ such that `battery life_j > battery life_i` and `torque_j > torque_i`.

Your task is to return the number of weaker robots.

## Examples

### 1

#### Input
3
5 5
6 3
3 6

#### Output
0

#### Explanation
No robot has strictly greater battery life and torque than another.

### 2

#### Input
2
2 2
3 3

#### Output
1

#### Explanation
The first robot (2, 2) is weaker because the second robot (3, 3) has strictly greater battery life and torque.

## Input Format
- The first line contains an integer $n$, the number of robots.
- The next $n$ lines each contain two space-separated integers, representing the battery life and torque of a robot.

## Output Format
- Return a single integer representing the number of weaker robots.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ battery life, torque ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy, sorting
