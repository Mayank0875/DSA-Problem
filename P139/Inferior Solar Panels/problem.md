## Title
Inferior Solar Panels

## Slug
inferior-solar-panels

## Difficulty
Medium

## Description
An energy firm tests solar panels.

You have a list of $n$ panels. Each panel has two main properties: **energy output** and **lifespan**. You are given a 2D integer array `properties` where `properties[i] = [energy output_i, lifespan_i]` represents the attributes of the $i$-th panel.

A panel is considered **inferior** if there exists another panel that has **both** strictly greater energy output and strictly greater lifespan.

More formally, the $i$-th panel is inferior if there exists an index $j$ such that `energy output_j > energy output_i` and `lifespan_j > lifespan_i`.

Your task is to return the number of inferior panels.

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
No panel has strictly greater energy output and lifespan than another.

### 2

#### Input
2
2 2
3 3

#### Output
1

#### Explanation
The first panel (2, 2) is inferior because the second panel (3, 3) has strictly greater energy output and lifespan.

## Input Format
- The first line contains an integer $n$, the number of panels.
- The next $n$ lines each contain two space-separated integers, representing the energy output and lifespan of a panel.

## Output Format
- Return a single integer representing the number of inferior panels.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ energy output, lifespan ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy, sorting
