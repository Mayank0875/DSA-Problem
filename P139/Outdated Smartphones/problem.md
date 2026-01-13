## Title
Outdated Smartphones

## Slug
outdated-smartphones

## Difficulty
Medium

## Description
A review site compares phone models.

You have a list of $n$ phones. Each phone has two main properties: **battery life** and **camera resolution**. You are given a 2D integer array `properties` where `properties[i] = [battery life_i, camera resolution_i]` represents the attributes of the $i$-th phone.

A phone is considered **outdated** if there exists another phone that has **both** strictly greater battery life and strictly greater camera resolution.

More formally, the $i$-th phone is outdated if there exists an index $j$ such that `battery life_j > battery life_i` and `camera resolution_j > camera resolution_i`.

Your task is to return the number of outdated phones.

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
No phone has strictly greater battery life and camera resolution than another.

### 2

#### Input
2
2 2
3 3

#### Output
1

#### Explanation
The first phone (2, 2) is outdated because the second phone (3, 3) has strictly greater battery life and camera resolution.

## Input Format
- The first line contains an integer $n$, the number of phones.
- The next $n$ lines each contain two space-separated integers, representing the battery life and camera resolution of a phone.

## Output Format
- Return a single integer representing the number of outdated phones.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ battery life, camera resolution ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy, sorting
