## Title
Obsolete Laptops

## Slug
obsolete-laptops

## Difficulty
Medium

## Description
A tech store tracks laptop performance.

You have a list of $n$ laptops. Each laptop has two main properties: **processor speed** and **RAM size**. You are given a 2D integer array `properties` where `properties[i] = [processor speed_i, RAM size_i]` represents the attributes of the $i$-th laptop.

A laptop is considered **obsolete** if there exists another laptop that has **both** strictly greater processor speed and strictly greater RAM size.

More formally, the $i$-th laptop is obsolete if there exists an index $j$ such that `processor speed_j > processor speed_i` and `RAM size_j > RAM size_i`.

Your task is to return the number of obsolete laptops.

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
No laptop has strictly greater processor speed and RAM size than another.

### 2

#### Input
2
2 2
3 3

#### Output
1

#### Explanation
The first laptop (2, 2) is obsolete because the second laptop (3, 3) has strictly greater processor speed and RAM size.

## Input Format
- The first line contains an integer $n$, the number of laptops.
- The next $n$ lines each contain two space-separated integers, representing the processor speed and RAM size of a laptop.

## Output Format
- Return a single integer representing the number of obsolete laptops.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ processor speed, RAM size ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy, sorting
