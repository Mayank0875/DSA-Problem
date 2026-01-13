## Title
Slower Trains

## Slug
slower-trains

## Difficulty
Medium

## Description
A railway operator schedules trains.

You have a list of $n$ trains. Each train has two main properties: **cargo capacity** and **max speed**. You are given a 2D integer array `properties` where `properties[i] = [cargo capacity_i, max speed_i]` represents the attributes of the $i$-th train.

A train is considered **slower** if there exists another train that has **both** strictly greater cargo capacity and strictly greater max speed.

More formally, the $i$-th train is slower if there exists an index $j$ such that `cargo capacity_j > cargo capacity_i` and `max speed_j > max speed_i`.

Your task is to return the number of slower trains.

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
No train has strictly greater cargo capacity and max speed than another.

### 2

#### Input
2
2 2
3 3

#### Output
1

#### Explanation
The first train (2, 2) is slower because the second train (3, 3) has strictly greater cargo capacity and max speed.

## Input Format
- The first line contains an integer $n$, the number of trains.
- The next $n$ lines each contain two space-separated integers, representing the cargo capacity and max speed of a train.

## Output Format
- Return a single integer representing the number of slower trains.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ cargo capacity, max speed ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy, sorting
