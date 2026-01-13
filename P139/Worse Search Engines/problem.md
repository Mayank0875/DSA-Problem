## Title
Worse Search Engines

## Slug
worse-search-engines

## Difficulty
Medium

## Description
A tech analyst tests search algorithms.

You have a list of $n$ engines. Each engine has two main properties: **index size** and **query speed**. You are given a 2D integer array `properties` where `properties[i] = [index size_i, query speed_i]` represents the attributes of the $i$-th engine.

A engine is considered **worse** if there exists another engine that has **both** strictly greater index size and strictly greater query speed.

More formally, the $i$-th engine is worse if there exists an index $j$ such that `index size_j > index size_i` and `query speed_j > query speed_i`.

Your task is to return the number of worse engines.

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
No engine has strictly greater index size and query speed than another.

### 2

#### Input
2
2 2
3 3

#### Output
1

#### Explanation
The first engine (2, 2) is worse because the second engine (3, 3) has strictly greater index size and query speed.

## Input Format
- The first line contains an integer $n$, the number of engines.
- The next $n$ lines each contain two space-separated integers, representing the index size and query speed of a engine.

## Output Format
- Return a single integer representing the number of worse engines.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ index size, query speed ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy, sorting
