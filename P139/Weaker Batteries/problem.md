## Title
Weaker Batteries

## Slug
weaker-batteries

## Difficulty
Medium

## Description
An engineer tests battery cells.

You have a list of $n$ batteries. Each battery has two main properties: **capacity (mAh)** and **charge rate**. You are given a 2D integer array `properties` where `properties[i] = [capacity (mAh)_i, charge rate_i]` represents the attributes of the $i$-th battery.

A battery is considered **weaker** if there exists another battery that has **both** strictly greater capacity (mAh) and strictly greater charge rate.

More formally, the $i$-th battery is weaker if there exists an index $j$ such that `capacity (mAh)_j > capacity (mAh)_i` and `charge rate_j > charge rate_i`.

Your task is to return the number of weaker batteries.

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
No battery has strictly greater capacity (mAh) and charge rate than another.

### 2

#### Input
2
2 2
3 3

#### Output
1

#### Explanation
The first battery (2, 2) is weaker because the second battery (3, 3) has strictly greater capacity (mAh) and charge rate.

## Input Format
- The first line contains an integer $n$, the number of batteries.
- The next $n$ lines each contain two space-separated integers, representing the capacity (mAh) and charge rate of a battery.

## Output Format
- Return a single integer representing the number of weaker batteries.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ capacity (mAh), charge rate ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy, sorting
