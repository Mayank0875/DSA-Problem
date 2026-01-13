## Title
Worse Fire Extinguishers

## Slug
worse-fire-extinguishers

## Difficulty
Medium

## Description
A safety inspector checks equipment.

You have a list of $n$ extinguishers. Each extinguisher has two main properties: **capacity** and **discharge range**. You are given a 2D integer array `properties` where `properties[i] = [capacity_i, discharge range_i]` represents the attributes of the $i$-th extinguisher.

A extinguisher is considered **worse** if there exists another extinguisher that has **both** strictly greater capacity and strictly greater discharge range.

More formally, the $i$-th extinguisher is worse if there exists an index $j$ such that `capacity_j > capacity_i` and `discharge range_j > discharge range_i`.

Your task is to return the number of worse extinguishers.

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
No extinguisher has strictly greater capacity and discharge range than another.

### 2

#### Input
2
2 2
3 3

#### Output
1

#### Explanation
The first extinguisher (2, 2) is worse because the second extinguisher (3, 3) has strictly greater capacity and discharge range.

## Input Format
- The first line contains an integer $n$, the number of extinguishers.
- The next $n$ lines each contain two space-separated integers, representing the capacity and discharge range of a extinguisher.

## Output Format
- Return a single integer representing the number of worse extinguishers.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ capacity, discharge range ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy, sorting
