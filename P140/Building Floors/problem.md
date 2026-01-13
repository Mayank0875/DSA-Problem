## Title
Building Floors

## Slug
building-floors

## Difficulty
Easy

## Description
An architect compares the height of skyscrapers in a skyline.

The blueprint data records the floor count of $N$ buildings in an array. To visualize the skyline, the architect needs to assign a rank to every building based on its floor count.

The ranking rules are simple: the building with the **smallest** floor count gets **Rank 1**. The next distinct floor count gets **Rank 2**, and so on.

If two or more buildings have the exact same floor count, they must receive the **same rank**. The ranks must be integers starting from 1.

Your task is to replace each building's floor count with its corresponding rank.

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
All buildings share the same floor count, so they share Rank 1.

## Input Format
- The first line contains an integer `n`, the number of buildings.
- The second line contains `n` space-separated integers representing the floor counts.

## Output Format
- Return an array of integers where each element is the rank of the corresponding building.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, sorting
