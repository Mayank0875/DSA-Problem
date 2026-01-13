## Title
Artifact Dating

## Slug
artifact-dating

## Difficulty
Easy

## Description
An archaeologist dates pottery shards by estimated year (negative for BC).

The carbon dating records the year of $N$ shards in an array. To build a timeline, the archaeologist needs to assign a rank to every shard based on its year.

The ranking rules are simple: the shard with the **smallest** year gets **Rank 1**. The next distinct year gets **Rank 2**, and so on.

If two or more shards have the exact same year, they must receive the **same rank**. The ranks must be integers starting from 1.

Your task is to replace each shard's year with its corresponding rank.

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
All shards share the same year, so they share Rank 1.

## Input Format
- The first line contains an integer `n`, the number of shards.
- The second line contains `n` space-separated integers representing the years.

## Output Format
- Return an array of integers where each element is the rank of the corresponding shard.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, sorting
