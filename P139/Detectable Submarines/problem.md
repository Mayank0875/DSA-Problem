## Title
Detectable Submarines

## Slug
detectable-submarines

## Difficulty
Medium

## Description
A navy tests stealth subs.

You have a list of $n$ submarines. Each submarine has two main properties: **max depth** and **stealth rating**. You are given a 2D integer array `properties` where `properties[i] = [max depth_i, stealth rating_i]` represents the attributes of the $i$-th submarine.

A submarine is considered **detectable** if there exists another submarine that has **both** strictly greater max depth and strictly greater stealth rating.

More formally, the $i$-th submarine is detectable if there exists an index $j$ such that `max depth_j > max depth_i` and `stealth rating_j > stealth rating_i`.

Your task is to return the number of detectable submarines.

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
No submarine has strictly greater max depth and stealth rating than another.

### 2

#### Input
2
2 2
3 3

#### Output
1

#### Explanation
The first submarine (2, 2) is detectable because the second submarine (3, 3) has strictly greater max depth and stealth rating.

## Input Format
- The first line contains an integer $n$, the number of submarines.
- The next $n$ lines each contain two space-separated integers, representing the max depth and stealth rating of a submarine.

## Output Format
- Return a single integer representing the number of detectable submarines.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ max depth, stealth rating ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy, sorting
