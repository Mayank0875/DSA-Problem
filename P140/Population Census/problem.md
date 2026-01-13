## Title
Population Census

## Slug
population-census

## Difficulty
Easy

## Description
A government ranks towns by population size.

The census data records the population of $N$ towns in an array. To allocate funds, the official needs to assign a rank to every town based on its population.

The ranking rules are simple: the town with the **smallest** population gets **Rank 1**. The next distinct population gets **Rank 2**, and so on.

If two or more towns have the exact same population, they must receive the **same rank**. The ranks must be integers starting from 1.

Your task is to replace each town's population with its corresponding rank.

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
All towns share the same population, so they share Rank 1.

## Input Format
- The first line contains an integer `n`, the number of towns.
- The second line contains `n` space-separated integers representing the populations.

## Output Format
- Return an array of integers where each element is the rank of the corresponding town.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, sorting
