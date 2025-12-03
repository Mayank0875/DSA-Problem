## Title
Chemical Synthesis

## Slug
chemical-synthesis

## Difficulty
Medium

## Description
A chemical reaction starts with a base compound (1) and goes through intermediate stages to form the final product (n). Each reaction step is irreversible.

There are n compounds numbered from 1 to n.
    1. Compound 1 is the starting point.
    2. Compound n is the destination.

Between some compounds, there are one-way reactions that allow movement from u to v. The system contains no loops (directed acyclic graph), meaning you can only move forward towards the goal.

Your task is to find the total number of distinct ways/paths to travel from Compound 1 to Compound n. Since the answer can be very large, return the count modulo 1000000007.

## Examples

### 1

#### Input
4 5
1 2
2 4
1 3
3 4
1 4

#### Output
3

#### Explanation
There are 3 distinct paths:
1 -> 2 -> 4
1 -> 3 -> 4
1 -> 4

### 2

#### Input
4 5
1 2
3 4
2 3
1 3
2 4

#### Output
3

#### Explanation
There are 3 distinct paths:
1 -> 2 -> 3 -> 4
1 -> 2 -> 4
1 -> 3 -> 4

## Input Format
- The first line contains two integers n and m: the number of compounds and the number of reactions.
- The next m lines each contain two integers u and v, representing a one-way reaction from u to v.

## Output Format
- Return a single integer: the number of ways to travel from 1 to n, modulo (1e9 + 7).

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ m ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, dynamic-programming
