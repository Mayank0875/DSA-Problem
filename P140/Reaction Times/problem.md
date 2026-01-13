## Title
Reaction Times

## Slug
reaction-times

## Difficulty
Easy

## Description
Athletes test their reflexes. Lower time means better rank.

The test records the reaction time (ms) of $N$ athletes in an array. To assess agility, the coach needs to assign a rank to every athlete based on its reaction time (ms).

The ranking rules are simple: the athlete with the **smallest** reaction time (ms) gets **Rank 1**. The next distinct reaction time (ms) gets **Rank 2**, and so on.

If two or more athletes have the exact same reaction time (ms), they must receive the **same rank**. The ranks must be integers starting from 1.

Your task is to replace each athlete's reaction time (ms) with its corresponding rank.

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
All athletes share the same reaction time (ms), so they share Rank 1.

## Input Format
- The first line contains an integer `n`, the number of athletes.
- The second line contains `n` space-separated integers representing the reaction time (ms)s.

## Output Format
- Return an array of integers where each element is the rank of the corresponding athlete.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, sorting
