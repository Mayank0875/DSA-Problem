## Title
Inefficient Factories

## Slug
inefficient-factories

## Difficulty
Medium

## Description
A corporation evaluates manufacturing plants.

You have a list of $n$ factories. Each factory has two main properties: **production rate** and **efficiency score**. You are given a 2D integer array `properties` where `properties[i] = [production rate_i, efficiency score_i]` represents the attributes of the $i$-th factory.

A factory is considered **inefficient** if there exists another factory that has **both** strictly greater production rate and strictly greater efficiency score.

More formally, the $i$-th factory is inefficient if there exists an index $j$ such that `production rate_j > production rate_i` and `efficiency score_j > efficiency score_i`.

Your task is to return the number of inefficient factories.

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
No factory has strictly greater production rate and efficiency score than another.

### 2

#### Input
2
2 2
3 3

#### Output
1

#### Explanation
The first factory (2, 2) is inefficient because the second factory (3, 3) has strictly greater production rate and efficiency score.

## Input Format
- The first line contains an integer $n$, the number of factories.
- The next $n$ lines each contain two space-separated integers, representing the production rate and efficiency score of a factory.

## Output Format
- Return a single integer representing the number of inefficient factories.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ production rate, efficiency score ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy, sorting
