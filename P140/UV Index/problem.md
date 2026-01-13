## Title
UV Index

## Slug
uv-index

## Difficulty
Easy

## Description
A beach safety team monitors UV radiation levels.

The sensor reading records the UV index of $N$ hours in an array. To update the warnings, the lifeguard needs to assign a rank to every hour based on its UV index.

The ranking rules are simple: the hour with the **smallest** UV index gets **Rank 1**. The next distinct UV index gets **Rank 2**, and so on.

If two or more hours have the exact same UV index, they must receive the **same rank**. The ranks must be integers starting from 1.

Your task is to replace each hour's UV index with its corresponding rank.

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
All hours share the same UV index, so they share Rank 1.

## Input Format
- The first line contains an integer `n`, the number of hours.
- The second line contains `n` space-separated integers representing the UV indexs.

## Output Format
- Return an array of integers where each element is the rank of the corresponding hour.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, sorting
