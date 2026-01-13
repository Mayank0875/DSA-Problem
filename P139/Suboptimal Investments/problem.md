## Title
Suboptimal Investments

## Slug
suboptimal-investments

## Difficulty
Medium

## Description
An investor analyzes stock options.

You have a list of $n$ stocks. Each stock has two main properties: **return rate** and **safety rating**. You are given a 2D integer array `properties` where `properties[i] = [return rate_i, safety rating_i]` represents the attributes of the $i$-th stock.

A stock is considered **suboptimal** if there exists another stock that has **both** strictly greater return rate and strictly greater safety rating.

More formally, the $i$-th stock is suboptimal if there exists an index $j$ such that `return rate_j > return rate_i` and `safety rating_j > safety rating_i`.

Your task is to return the number of suboptimal stocks.

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
No stock has strictly greater return rate and safety rating than another.

### 2

#### Input
2
2 2
3 3

#### Output
1

#### Explanation
The first stock (2, 2) is suboptimal because the second stock (3, 3) has strictly greater return rate and safety rating.

## Input Format
- The first line contains an integer $n$, the number of stocks.
- The next $n$ lines each contain two space-separated integers, representing the return rate and safety rating of a stock.

## Output Format
- Return a single integer representing the number of suboptimal stocks.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ return rate, safety rating ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy, sorting
