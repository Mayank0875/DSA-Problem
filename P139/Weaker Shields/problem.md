## Title
Weaker Shields

## Slug
weaker-shields

## Difficulty
Medium

## Description
A blacksmith evaluates shields.

You have a list of $n$ shields. Each shield has two main properties: **durability** and **block chance**. You are given a 2D integer array `properties` where `properties[i] = [durability_i, block chance_i]` represents the attributes of the $i$-th shield.

A shield is considered **weaker** if there exists another shield that has **both** strictly greater durability and strictly greater block chance.

More formally, the $i$-th shield is weaker if there exists an index $j$ such that `durability_j > durability_i` and `block chance_j > block chance_i`.

Your task is to return the number of weaker shields.

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
No shield has strictly greater durability and block chance than another.

### 2

#### Input
2
2 2
3 3

#### Output
1

#### Explanation
The first shield (2, 2) is weaker because the second shield (3, 3) has strictly greater durability and block chance.

## Input Format
- The first line contains an integer $n$, the number of shields.
- The next $n$ lines each contain two space-separated integers, representing the durability and block chance of a shield.

## Output Format
- Return a single integer representing the number of weaker shields.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ durability, block chance ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy, sorting
