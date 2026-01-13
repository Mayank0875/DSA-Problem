## Title
Planet Distances

## Slug
planet-distances

## Difficulty
Easy

## Description
An astronomer ranks exoplanets based on their distance from Earth.

The telescope records the distance (light years) of $N$ planets in an array. To prioritize exploration, the researcher needs to assign a rank to every planet based on its distance (light years).

The ranking rules are simple: the planet with the **smallest** distance (light years) gets **Rank 1**. The next distinct distance (light years) gets **Rank 2**, and so on.

If two or more planets have the exact same distance (light years), they must receive the **same rank**. The ranks must be integers starting from 1.

Your task is to replace each planet's distance (light years) with its corresponding rank.

## Examples

### 1

#### Input
4
40 10 20 30

#### Output
4 1 2 3

#### Explanation
10 is the smallest (Rank 1). 20 is the second smallest (Rank 2). 30 is third (Rank 3). 40 is largest (Rank 4).

### 2

#### Input
3
2 2 2

#### Output
1 1 1

#### Explanation
All planets share the same distance (light years), so they share Rank 1.

## Input Format
- The first line contains an integer `n`, the number of planets.
- The second line contains `n` space-separated integers representing the distance (light years)s.

## Output Format
- Return an array of integers where each element is the rank of the corresponding planet.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, sorting
