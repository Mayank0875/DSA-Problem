## Title
Weaker Bridges

## Slug
weaker-bridges

## Difficulty
Medium

## Description
Civil engineers inspect bridge designs.

You have a list of $n$ bridges. Each bridge has two main properties: **load limit** and **span length**. You are given a 2D integer array `properties` where `properties[i] = [load limit_i, span length_i]` represents the attributes of the $i$-th bridge.

A bridge is considered **weaker** if there exists another bridge that has **both** strictly greater load limit and strictly greater span length.

More formally, the $i$-th bridge is weaker if there exists an index $j$ such that `load limit_j > load limit_i` and `span length_j > span length_i`.

Your task is to return the number of weaker bridges.

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
No bridge has strictly greater load limit and span length than another.

### 2

#### Input
2
2 2
3 3

#### Output
1

#### Explanation
The first bridge (2, 2) is weaker because the second bridge (3, 3) has strictly greater load limit and span length.

## Input Format
- The first line contains an integer $n$, the number of bridges.
- The next $n$ lines each contain two space-separated integers, representing the load limit and span length of a bridge.

## Output Format
- Return a single integer representing the number of weaker bridges.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ load limit, span length ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy, sorting
