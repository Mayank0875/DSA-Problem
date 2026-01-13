## Title
Worse Elevators

## Slug
worse-elevators

## Difficulty
Medium

## Description
A building manager inspects elevators.

You have a list of $n$ elevators. Each elevator has two main properties: **capacity** and **speed**. You are given a 2D integer array `properties` where `properties[i] = [capacity_i, speed_i]` represents the attributes of the $i$-th elevator.

A elevator is considered **worse** if there exists another elevator that has **both** strictly greater capacity and strictly greater speed.

More formally, the $i$-th elevator is worse if there exists an index $j$ such that `capacity_j > capacity_i` and `speed_j > speed_i`.

Your task is to return the number of worse elevators.

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
No elevator has strictly greater capacity and speed than another.

### 2

#### Input
2
2 2
3 3

#### Output
1

#### Explanation
The first elevator (2, 2) is worse because the second elevator (3, 3) has strictly greater capacity and speed.

## Input Format
- The first line contains an integer $n$, the number of elevators.
- The next $n$ lines each contain two space-separated integers, representing the capacity and speed of a elevator.

## Output Format
- Return a single integer representing the number of worse elevators.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ capacity, speed ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy, sorting
