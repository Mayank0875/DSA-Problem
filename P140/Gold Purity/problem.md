## Title
Gold Purity

## Slug
gold-purity

## Difficulty
Easy

## Description
A pawn shop checks the karat value of jewelry.

The acid test records the karat of $N$ rings in an array. To value the items, the broker needs to assign a rank to every ring based on its karat.

The ranking rules are simple: the ring with the **smallest** karat gets **Rank 1**. The next distinct karat gets **Rank 2**, and so on.

If two or more rings have the exact same karat, they must receive the **same rank**. The ranks must be integers starting from 1.

Your task is to replace each ring's karat with its corresponding rank.

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
All rings share the same karat, so they share Rank 1.

## Input Format
- The first line contains an integer `n`, the number of rings.
- The second line contains `n` space-separated integers representing the karats.

## Output Format
- Return an array of integers where each element is the rank of the corresponding ring.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, sorting
