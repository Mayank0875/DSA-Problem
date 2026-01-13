## Title
Less Powerful Telescopes

## Slug
less-powerful-telescopes

## Difficulty
Medium

## Description
An observatory ranks telescopes.

You have a list of $n$ telescopes. Each telescope has two main properties: **aperture size** and **focal length**. You are given a 2D integer array `properties` where `properties[i] = [aperture size_i, focal length_i]` represents the attributes of the $i$-th telescope.

A telescope is considered **less powerful** if there exists another telescope that has **both** strictly greater aperture size and strictly greater focal length.

More formally, the $i$-th telescope is less powerful if there exists an index $j$ such that `aperture size_j > aperture size_i` and `focal length_j > focal length_i`.

Your task is to return the number of less powerful telescopes.

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
No telescope has strictly greater aperture size and focal length than another.

### 2

#### Input
2
2 2
3 3

#### Output
1

#### Explanation
The first telescope (2, 2) is less powerful because the second telescope (3, 3) has strictly greater aperture size and focal length.

## Input Format
- The first line contains an integer $n$, the number of telescopes.
- The next $n$ lines each contain two space-separated integers, representing the aperture size and focal length of a telescope.

## Output Format
- Return a single integer representing the number of less powerful telescopes.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ aperture size, focal length ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy, sorting
