## Title
Rainfall Amount

## Slug
rainfall-amount

## Difficulty
Easy

## Description
A hydrologist records rainfall in different districts.

The rain gauge records the rainfall (mm) of $N$ districts in an array. To predict flooding, the hydrologist needs to assign a rank to every district based on its rainfall (mm).

The ranking rules are simple: the district with the **smallest** rainfall (mm) gets **Rank 1**. The next distinct rainfall (mm) gets **Rank 2**, and so on.

If two or more districts have the exact same rainfall (mm), they must receive the **same rank**. The ranks must be integers starting from 1.

Your task is to replace each district's rainfall (mm) with its corresponding rank.

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
All districts share the same rainfall (mm), so they share Rank 1.

## Input Format
- The first line contains an integer `n`, the number of districts.
- The second line contains `n` space-separated integers representing the rainfall (mm)s.

## Output Format
- Return an array of integers where each element is the rank of the corresponding district.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, sorting
