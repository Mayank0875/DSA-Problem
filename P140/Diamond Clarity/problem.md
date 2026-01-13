## Title
Diamond Clarity

## Slug
diamond-clarity

## Difficulty
Easy

## Description
A jeweler sorts diamonds. Lower flaw counts mean better clarity ranks.

The microscope analysis records the flaw count of $N$ diamonds in an array. To price the gems, the jeweler needs to assign a rank to every diamond based on its flaw count.

The ranking rules are simple: the diamond with the **smallest** flaw count gets **Rank 1**. The next distinct flaw count gets **Rank 2**, and so on.

If two or more diamonds have the exact same flaw count, they must receive the **same rank**. The ranks must be integers starting from 1.

Your task is to replace each diamond's flaw count with its corresponding rank.

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
All diamonds share the same flaw count, so they share Rank 1.

## Input Format
- The first line contains an integer `n`, the number of diamonds.
- The second line contains `n` space-separated integers representing the flaw counts.

## Output Format
- Return an array of integers where each element is the rank of the corresponding diamond.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, sorting
