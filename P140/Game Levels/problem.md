## Title
Game Levels

## Slug
game-levels

## Difficulty
Easy

## Description
A player unlocks levels. The game displays them by difficulty rating.

The menu records the difficulty rating of $N$ levels in an array. To choose a challenge, the player needs to assign a rank to every level based on its difficulty rating.

The ranking rules are simple: the level with the **smallest** difficulty rating gets **Rank 1**. The next distinct difficulty rating gets **Rank 2**, and so on.

If two or more levels have the exact same difficulty rating, they must receive the **same rank**. The ranks must be integers starting from 1.

Your task is to replace each level's difficulty rating with its corresponding rank.

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
All levels share the same difficulty rating, so they share Rank 1.

## Input Format
- The first line contains an integer `n`, the number of levels.
- The second line contains `n` space-separated integers representing the difficulty ratings.

## Output Format
- Return an array of integers where each element is the rank of the corresponding level.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, sorting
