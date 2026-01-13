## Title
Raju's Kite Festival

## Slug
rajus-kite-festival

## Difficulty
Easy

## Description
Raju is organizing a grand Patang (kite) festival in his village.

Raju records the flying height of $N$ kites in an array. To declare the results, he needs to assign a rank to every kite based on its flying height.

The ranking rules are simple: the kite with the **smallest** flying height gets **Rank 1**. The next distinct flying height gets **Rank 2**, and so on.

If two or more kites have the exact same flying height, they must receive the **same rank**. The ranks must be integers starting from 1.

Your task is to replace each kite's flying height with its corresponding rank.

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
All kites share the same flying height, so they share Rank 1.

## Input Format
- The first line contains an integer `n`, the number of kites.
- The second line contains `n` space-separated integers representing the flying heights.

## Output Format
- Return an array of integers where each element is the rank of the corresponding kite.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, sorting
