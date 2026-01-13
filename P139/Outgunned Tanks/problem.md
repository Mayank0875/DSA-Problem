## Title
Outgunned Tanks

## Slug
outgunned-tanks

## Difficulty
Medium

## Description
A military sim compares tank models.

You have a list of $n$ tanks. Each tank has two main properties: **armor thickness** and **firepower**. You are given a 2D integer array `properties` where `properties[i] = [armor thickness_i, firepower_i]` represents the attributes of the $i$-th tank.

A tank is considered **outgunned** if there exists another tank that has **both** strictly greater armor thickness and strictly greater firepower.

More formally, the $i$-th tank is outgunned if there exists an index $j$ such that `armor thickness_j > armor thickness_i` and `firepower_j > firepower_i`.

Your task is to return the number of outgunned tanks.

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
No tank has strictly greater armor thickness and firepower than another.

### 2

#### Input
2
2 2
3 3

#### Output
1

#### Explanation
The first tank (2, 2) is outgunned because the second tank (3, 3) has strictly greater armor thickness and firepower.

## Input Format
- The first line contains an integer $n$, the number of tanks.
- The next $n$ lines each contain two space-separated integers, representing the armor thickness and firepower of a tank.

## Output Format
- Return a single integer representing the number of outgunned tanks.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ armor thickness, firepower ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy, sorting
