## Title
Coffee Roast

## Slug
coffee-roast

## Difficulty
Easy

## Description
A roaster classifies beans by roast level (1=light, higher=darker).

The roaster log records the roast level of $N$ batches in an array. To label the bags, the master roaster needs to assign a rank to every batch based on its roast level.

The ranking rules are simple: the batch with the **smallest** roast level gets **Rank 1**. The next distinct roast level gets **Rank 2**, and so on.

If two or more batches have the exact same roast level, they must receive the **same rank**. The ranks must be integers starting from 1.

Your task is to replace each batch's roast level with its corresponding rank.

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
All batches share the same roast level, so they share Rank 1.

## Input Format
- The first line contains an integer `n`, the number of batches.
- The second line contains `n` space-separated integers representing the roast levels.

## Output Format
- Return an array of integers where each element is the rank of the corresponding batch.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, sorting
