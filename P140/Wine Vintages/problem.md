## Title
Wine Vintages

## Slug
wine-vintages

## Difficulty
Easy

## Description
A sommelier organizes wines by year of production.

The cellar log records the year of $N$ wines in an array. To sort the cellar, the sommelier needs to assign a rank to every wine based on its year.

The ranking rules are simple: the wine with the **smallest** year gets **Rank 1**. The next distinct year gets **Rank 2**, and so on.

If two or more wines have the exact same year, they must receive the **same rank**. The ranks must be integers starting from 1.

Your task is to replace each wine's year with its corresponding rank.

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
All wines share the same year, so they share Rank 1.

## Input Format
- The first line contains an integer `n`, the number of wines.
- The second line contains `n` space-separated integers representing the years.

## Output Format
- Return an array of integers where each element is the rank of the corresponding wine.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, sorting
