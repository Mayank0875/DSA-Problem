## Title
Inferior Armor

## Slug
inferior-armor

## Difficulty
Medium

## Description
A knight chooses armor sets.

You have a list of $n$ armors. Each armor set has two main properties: **physical defense** and **magic resistance**. You are given a 2D integer array `properties` where `properties[i] = [physical defense_i, magic resistance_i]` represents the attributes of the $i$-th armor set.

A armor set is considered **inferior** if there exists another armor set that has **both** strictly greater physical defense and strictly greater magic resistance.

More formally, the $i$-th armor set is inferior if there exists an index $j$ such that `physical defense_j > physical defense_i` and `magic resistance_j > magic resistance_i`.

Your task is to return the number of inferior armors.

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
No armor set has strictly greater physical defense and magic resistance than another.

### 2

#### Input
2
2 2
3 3

#### Output
1

#### Explanation
The first armor set (2, 2) is inferior because the second armor set (3, 3) has strictly greater physical defense and magic resistance.

## Input Format
- The first line contains an integer $n$, the number of armors.
- The next $n$ lines each contain two space-separated integers, representing the physical defense and magic resistance of a armor set.

## Output Format
- Return a single integer representing the number of inferior armors.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ physical defense, magic resistance ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy, sorting
