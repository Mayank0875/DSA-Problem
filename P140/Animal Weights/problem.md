## Title
Animal Weights

## Slug
animal-weights

## Difficulty
Easy

## Description
A zoo checks the health of animals by tracking their weight.

The scale records the weight (kg) of $N$ animals in an array. To assess health, the vet needs to assign a rank to every animal based on its weight (kg).

The ranking rules are simple: the animal with the **smallest** weight (kg) gets **Rank 1**. The next distinct weight (kg) gets **Rank 2**, and so on.

If two or more animals have the exact same weight (kg), they must receive the **same rank**. The ranks must be integers starting from 1.

Your task is to replace each animal's weight (kg) with its corresponding rank.

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
All animals share the same weight (kg), so they share Rank 1.

## Input Format
- The first line contains an integer `n`, the number of animals.
- The second line contains `n` space-separated integers representing the weight (kg)s.

## Output Format
- Return an array of integers where each element is the rank of the corresponding animal.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, sorting
