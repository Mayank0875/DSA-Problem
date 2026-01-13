## Title
Hard Drive Storage

## Slug
hard-drive-storage

## Difficulty
Easy

## Description
An IT manager inventories drives by capacity.

The asset log records the capacity (GB) of $N$ drives in an array. To plan upgrades, the manager needs to assign a rank to every drive based on its capacity (GB).

The ranking rules are simple: the drive with the **smallest** capacity (GB) gets **Rank 1**. The next distinct capacity (GB) gets **Rank 2**, and so on.

If two or more drives have the exact same capacity (GB), they must receive the **same rank**. The ranks must be integers starting from 1.

Your task is to replace each drive's capacity (GB) with its corresponding rank.

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
All drives share the same capacity (GB), so they share Rank 1.

## Input Format
- The first line contains an integer `n`, the number of drives.
- The second line contains `n` space-separated integers representing the capacity (GB)s.

## Output Format
- Return an array of integers where each element is the rank of the corresponding drive.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, sorting
