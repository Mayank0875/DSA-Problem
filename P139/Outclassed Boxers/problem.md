## Title
Outclassed Boxers

## Slug
outclassed-boxers

## Difficulty
Medium

## Description
A boxing league ranks fighters.

You have a list of $n$ boxers. Each boxer has two main properties: **strength** and **agility**. You are given a 2D integer array `properties` where `properties[i] = [strength_i, agility_i]` represents the attributes of the $i$-th boxer.

A boxer is considered **outclassed** if there exists another boxer that has **both** strictly greater strength and strictly greater agility.

More formally, the $i$-th boxer is outclassed if there exists an index $j$ such that `strength_j > strength_i` and `agility_j > agility_i`.

Your task is to return the number of outclassed boxers.

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
No boxer has strictly greater strength and agility than another.

### 2

#### Input
2
2 2
3 3

#### Output
1

#### Explanation
The first boxer (2, 2) is outclassed because the second boxer (3, 3) has strictly greater strength and agility.

## Input Format
- The first line contains an integer $n$, the number of boxers.
- The next $n$ lines each contain two space-separated integers, representing the strength and agility of a boxer.

## Output Format
- Return a single integer representing the number of outclassed boxers.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ strength, agility ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy, sorting
