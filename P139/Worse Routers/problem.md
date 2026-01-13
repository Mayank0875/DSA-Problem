## Title
Worse Routers

## Slug
worse-routers

## Difficulty
Medium

## Description
An ISP tests Wi-Fi routers.

You have a list of $n$ routers. Each router has two main properties: **coverage area** and **throughput speed**. You are given a 2D integer array `properties` where `properties[i] = [coverage area_i, throughput speed_i]` represents the attributes of the $i$-th router.

A router is considered **worse** if there exists another router that has **both** strictly greater coverage area and strictly greater throughput speed.

More formally, the $i$-th router is worse if there exists an index $j$ such that `coverage area_j > coverage area_i` and `throughput speed_j > throughput speed_i`.

Your task is to return the number of worse routers.

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
No router has strictly greater coverage area and throughput speed than another.

### 2

#### Input
2
2 2
3 3

#### Output
1

#### Explanation
The first router (2, 2) is worse because the second router (3, 3) has strictly greater coverage area and throughput speed.

## Input Format
- The first line contains an integer $n$, the number of routers.
- The next $n$ lines each contain two space-separated integers, representing the coverage area and throughput speed of a router.

## Output Format
- Return a single integer representing the number of worse routers.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ coverage area, throughput speed ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy, sorting
