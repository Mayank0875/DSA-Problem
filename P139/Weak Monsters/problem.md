## Title
Weak Monsters

## Slug
weak-monsters

## Difficulty
Medium

## Description
An RPG game spawns monsters.

You have a list of $n$ monsters. Each monster has two main properties: **health** and **damage**. You are given a 2D integer array `properties` where `properties[i] = [health_i, damage_i]` represents the attributes of the $i$-th monster.

A monster is considered **weak** if there exists another monster that has **both** strictly greater health and strictly greater damage.

More formally, the $i$-th monster is weak if there exists an index $j$ such that `health_j > health_i` and `damage_j > damage_i`.

Your task is to return the number of weak monsters.

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
No monster has strictly greater health and damage than another.

### 2

#### Input
2
2 2
3 3

#### Output
1

#### Explanation
The first monster (2, 2) is weak because the second monster (3, 3) has strictly greater health and damage.

## Input Format
- The first line contains an integer $n$, the number of monsters.
- The next $n$ lines each contain two space-separated integers, representing the health and damage of a monster.

## Output Format
- Return a single integer representing the number of weak monsters.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ health, damage ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy, sorting
