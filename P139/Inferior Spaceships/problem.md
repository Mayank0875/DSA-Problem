## Title
Inferior Spaceships

## Slug
inferior-spaceships

## Difficulty
Medium

## Description
A fleet admiral reviews ship specs.

You have a list of $n$ ships. Each ship has two main properties: **shield capacity** and **warp speed**. You are given a 2D integer array `properties` where `properties[i] = [shield capacity_i, warp speed_i]` represents the attributes of the $i$-th ship.

A ship is considered **inferior** if there exists another ship that has **both** strictly greater shield capacity and strictly greater warp speed.

More formally, the $i$-th ship is inferior if there exists an index $j$ such that `shield capacity_j > shield capacity_i` and `warp speed_j > warp speed_i`.

Your task is to return the number of inferior ships.

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
No ship has strictly greater shield capacity and warp speed than another.

### 2

#### Input
2
2 2
3 3

#### Output
1

#### Explanation
The first ship (2, 2) is inferior because the second ship (3, 3) has strictly greater shield capacity and warp speed.

## Input Format
- The first line contains an integer $n$, the number of ships.
- The next $n$ lines each contain two space-separated integers, representing the shield capacity and warp speed of a ship.

## Output Format
- Return a single integer representing the number of inferior ships.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ shield capacity, warp speed ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy, sorting
