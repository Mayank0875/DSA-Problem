## Title
Inferior Swords

## Slug
inferior-swords

## Difficulty
Medium

## Description
A warrior inspects weapons.

You have a list of $n$ swords. Each sword has two main properties: **damage** and **attack speed**. You are given a 2D integer array `properties` where `properties[i] = [damage_i, attack speed_i]` represents the attributes of the $i$-th sword.

A sword is considered **inferior** if there exists another sword that has **both** strictly greater damage and strictly greater attack speed.

More formally, the $i$-th sword is inferior if there exists an index $j$ such that `damage_j > damage_i` and `attack speed_j > attack speed_i`.

Your task is to return the number of inferior swords.

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
No sword has strictly greater damage and attack speed than another.

### 2

#### Input
2
2 2
3 3

#### Output
1

#### Explanation
The first sword (2, 2) is inferior because the second sword (3, 3) has strictly greater damage and attack speed.

## Input Format
- The first line contains an integer $n$, the number of swords.
- The next $n$ lines each contain two space-separated integers, representing the damage and attack speed of a sword.

## Output Format
- Return a single integer representing the number of inferior swords.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ damage, attack speed ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy, sorting
