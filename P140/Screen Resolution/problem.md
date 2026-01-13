## Title
Screen Resolution

## Slug
screen-resolution

## Difficulty
Easy

## Description
A tech reviewer compares monitors by total pixel count.

The spec sheet records the pixel count of $N$ monitors in an array. To rate clarity, the reviewer needs to assign a rank to every monitor based on its pixel count.

The ranking rules are simple: the monitor with the **smallest** pixel count gets **Rank 1**. The next distinct pixel count gets **Rank 2**, and so on.

If two or more monitors have the exact same pixel count, they must receive the **same rank**. The ranks must be integers starting from 1.

Your task is to replace each monitor's pixel count with its corresponding rank.

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
All monitors share the same pixel count, so they share Rank 1.

## Input Format
- The first line contains an integer `n`, the number of monitors.
- The second line contains `n` space-separated integers representing the pixel counts.

## Output Format
- Return an array of integers where each element is the rank of the corresponding monitor.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, sorting
