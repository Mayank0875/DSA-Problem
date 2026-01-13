## Title
Worse Cameras

## Slug
worse-cameras

## Difficulty
Medium

## Description
A photographer tests equipment.

You have a list of $n$ cameras. Each camera has two main properties: **ISO sensitivity** and **shutter speed**. You are given a 2D integer array `properties` where `properties[i] = [ISO sensitivity_i, shutter speed_i]` represents the attributes of the $i$-th camera.

A camera is considered **worse** if there exists another camera that has **both** strictly greater ISO sensitivity and strictly greater shutter speed.

More formally, the $i$-th camera is worse if there exists an index $j$ such that `ISO sensitivity_j > ISO sensitivity_i` and `shutter speed_j > shutter speed_i`.

Your task is to return the number of worse cameras.

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
No camera has strictly greater ISO sensitivity and shutter speed than another.

### 2

#### Input
2
2 2
3 3

#### Output
1

#### Explanation
The first camera (2, 2) is worse because the second camera (3, 3) has strictly greater ISO sensitivity and shutter speed.

## Input Format
- The first line contains an integer $n$, the number of cameras.
- The next $n$ lines each contain two space-separated integers, representing the ISO sensitivity and shutter speed of a camera.

## Output Format
- Return a single integer representing the number of worse cameras.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ ISO sensitivity, shutter speed ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy, sorting
