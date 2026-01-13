## Title
Smaller Planets

## Slug
smaller-planets

## Difficulty
Medium

## Description
An astronomer catalogs exoplanets.

You have a list of $n$ planets. Each planet has two main properties: **radius** and **mass**. You are given a 2D integer array `properties` where `properties[i] = [radius_i, mass_i]` represents the attributes of the $i$-th planet.

A planet is considered **smaller** if there exists another planet that has **both** strictly greater radius and strictly greater mass.

More formally, the $i$-th planet is smaller if there exists an index $j$ such that `radius_j > radius_i` and `mass_j > mass_i`.

Your task is to return the number of smaller planets.

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
No planet has strictly greater radius and mass than another.

### 2

#### Input
2
2 2
3 3

#### Output
1

#### Explanation
The first planet (2, 2) is smaller because the second planet (3, 3) has strictly greater radius and mass.

## Input Format
- The first line contains an integer $n$, the number of planets.
- The next $n$ lines each contain two space-separated integers, representing the radius and mass of a planet.

## Output Format
- Return a single integer representing the number of smaller planets.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ radius, mass ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy, sorting
