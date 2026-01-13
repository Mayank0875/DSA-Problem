## Title
Vitamin Dosage

## Slug
vitamin-dosage

## Difficulty
Easy

## Description
A pharmacist sorts supplements by dosage strength.

The inventory records the dosage (mg) of $N$ supplements in an array. To organize the shelf, the pharmacist needs to assign a rank to every supplement based on its dosage (mg).

The ranking rules are simple: the supplement with the **smallest** dosage (mg) gets **Rank 1**. The next distinct dosage (mg) gets **Rank 2**, and so on.

If two or more supplements have the exact same dosage (mg), they must receive the **same rank**. The ranks must be integers starting from 1.

Your task is to replace each supplement's dosage (mg) with its corresponding rank.

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
All supplements share the same dosage (mg), so they share Rank 1.

## Input Format
- The first line contains an integer `n`, the number of supplements.
- The second line contains `n` space-separated integers representing the dosage (mg)s.

## Output Format
- Return an array of integers where each element is the rank of the corresponding supplement.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, sorting
