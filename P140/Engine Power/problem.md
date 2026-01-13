## Title
Engine Power

## Slug
engine-power

## Difficulty
Easy

## Description
A car enthusiast compares engine horsepower.

The spec sheet records the horsepower of $N$ engines in an array. To find the strongest, the enthusiast needs to assign a rank to every engine based on its horsepower.

The ranking rules are simple: the engine with the **smallest** horsepower gets **Rank 1**. The next distinct horsepower gets **Rank 2**, and so on.

If two or more engines have the exact same horsepower, they must receive the **same rank**. The ranks must be integers starting from 1.

Your task is to replace each engine's horsepower with its corresponding rank.

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
All engines share the same horsepower, so they share Rank 1.

## Input Format
- The first line contains an integer `n`, the number of engines.
- The second line contains `n` space-separated integers representing the horsepowers.

## Output Format
- Return an array of integers where each element is the rank of the corresponding engine.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, sorting
