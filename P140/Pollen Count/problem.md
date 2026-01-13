## Title
Pollen Count

## Slug
pollen-count

## Difficulty
Easy

## Description
An allergy forecast ranks days by pollen levels.

The forecast records the pollen index of $N$ days in an array. To advise the public, the reporter needs to assign a rank to every day based on its pollen index.

The ranking rules are simple: the day with the **smallest** pollen index gets **Rank 1**. The next distinct pollen index gets **Rank 2**, and so on.

If two or more days have the exact same pollen index, they must receive the **same rank**. The ranks must be integers starting from 1.

Your task is to replace each day's pollen index with its corresponding rank.

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
All days share the same pollen index, so they share Rank 1.

## Input Format
- The first line contains an integer `n`, the number of days.
- The second line contains `n` space-separated integers representing the pollen indexs.

## Output Format
- Return an array of integers where each element is the rank of the corresponding day.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, sorting
