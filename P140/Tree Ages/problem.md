## Title
Tree Ages

## Slug
tree-ages

## Difficulty
Easy

## Description
A forester dates the trees in a grove using ring counts.

The survey records the age (years) of $N$ trees in an array. To study growth, the forester needs to assign a rank to every tree based on its age (years).

The ranking rules are simple: the tree with the **smallest** age (years) gets **Rank 1**. The next distinct age (years) gets **Rank 2**, and so on.

If two or more trees have the exact same age (years), they must receive the **same rank**. The ranks must be integers starting from 1.

Your task is to replace each tree's age (years) with its corresponding rank.

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
All trees share the same age (years), so they share Rank 1.

## Input Format
- The first line contains an integer `n`, the number of trees.
- The second line contains `n` space-separated integers representing the age (years)s.

## Output Format
- Return an array of integers where each element is the rank of the corresponding tree.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, sorting
