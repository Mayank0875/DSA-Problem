## Title
Slower Cars

## Slug
slower-cars

## Difficulty
Medium

## Description
A racing team compares car metrics.

You have a list of $n$ cars. Each car has two main properties: **top speed** and **acceleration**. You are given a 2D integer array `properties` where `properties[i] = [top speed_i, acceleration_i]` represents the attributes of the $i$-th car.

A car is considered **slower** if there exists another car that has **both** strictly greater top speed and strictly greater acceleration.

More formally, the $i$-th car is slower if there exists an index $j$ such that `top speed_j > top speed_i` and `acceleration_j > acceleration_i`.

Your task is to return the number of slower cars.

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
No car has strictly greater top speed and acceleration than another.

### 2

#### Input
2
2 2
3 3

#### Output
1

#### Explanation
The first car (2, 2) is slower because the second car (3, 3) has strictly greater top speed and acceleration.

## Input Format
- The first line contains an integer $n$, the number of cars.
- The next $n$ lines each contain two space-separated integers, representing the top speed and acceleration of a car.

## Output Format
- Return a single integer representing the number of slower cars.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ top speed, acceleration ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy, sorting
