## Title
Less Capable Drones

## Slug
less-capable-drones

## Difficulty
Medium

## Description
A surveillance firm tests drones.

You have a list of $n$ drones. Each drone has two main properties: **flight range** and **camera quality**. You are given a 2D integer array `properties` where `properties[i] = [flight range_i, camera quality_i]` represents the attributes of the $i$-th drone.

A drone is considered **less capable** if there exists another drone that has **both** strictly greater flight range and strictly greater camera quality.

More formally, the $i$-th drone is less capable if there exists an index $j$ such that `flight range_j > flight range_i` and `camera quality_j > camera quality_i`.

Your task is to return the number of less capable drones.

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
No drone has strictly greater flight range and camera quality than another.

### 2

#### Input
2
2 2
3 3

#### Output
1

#### Explanation
The first drone (2, 2) is less capable because the second drone (3, 3) has strictly greater flight range and camera quality.

## Input Format
- The first line contains an integer $n$, the number of drones.
- The next $n$ lines each contain two space-separated integers, representing the flight range and camera quality of a drone.

## Output Format
- Return a single integer representing the number of less capable drones.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ flight range, camera quality ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy, sorting
