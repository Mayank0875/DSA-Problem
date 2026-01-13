## Title
Weaker Microbes

## Slug
weaker-microbes

## Difficulty
Medium

## Description
A biologist studies virus strains.

You have a list of $n$ strains. Each strain has two main properties: **reproduction rate** and **drug resistance**. You are given a 2D integer array `properties` where `properties[i] = [reproduction rate_i, drug resistance_i]` represents the attributes of the $i$-th strain.

A strain is considered **weaker** if there exists another strain that has **both** strictly greater reproduction rate and strictly greater drug resistance.

More formally, the $i$-th strain is weaker if there exists an index $j$ such that `reproduction rate_j > reproduction rate_i` and `drug resistance_j > drug resistance_i`.

Your task is to return the number of weaker strains.

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
No strain has strictly greater reproduction rate and drug resistance than another.

### 2

#### Input
2
2 2
3 3

#### Output
1

#### Explanation
The first strain (2, 2) is weaker because the second strain (3, 3) has strictly greater reproduction rate and drug resistance.

## Input Format
- The first line contains an integer $n$, the number of strains.
- The next $n$ lines each contain two space-separated integers, representing the reproduction rate and drug resistance of a strain.

## Output Format
- Return a single integer representing the number of weaker strains.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ reproduction rate, drug resistance ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy, sorting
