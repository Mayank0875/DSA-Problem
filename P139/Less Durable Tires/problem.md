## Title
Less Durable Tires

## Slug
less-durable-tires

## Difficulty
Medium

## Description
A car mechanic compares tires.

You have a list of $n$ tires. Each tire has two main properties: **grip rating** and **tread life**. You are given a 2D integer array `properties` where `properties[i] = [grip rating_i, tread life_i]` represents the attributes of the $i$-th tire.

A tire is considered **less durable** if there exists another tire that has **both** strictly greater grip rating and strictly greater tread life.

More formally, the $i$-th tire is less durable if there exists an index $j$ such that `grip rating_j > grip rating_i` and `tread life_j > tread life_i`.

Your task is to return the number of less durable tires.

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
No tire has strictly greater grip rating and tread life than another.

### 2

#### Input
2
2 2
3 3

#### Output
1

#### Explanation
The first tire (2, 2) is less durable because the second tire (3, 3) has strictly greater grip rating and tread life.

## Input Format
- The first line contains an integer $n$, the number of tires.
- The next $n$ lines each contain two space-separated integers, representing the grip rating and tread life of a tire.

## Output Format
- Return a single integer representing the number of less durable tires.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ grip rating, tread life ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy, sorting
