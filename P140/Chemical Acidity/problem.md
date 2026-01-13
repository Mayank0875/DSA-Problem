## Title
Chemical Acidity

## Slug
chemical-acidity

## Difficulty
Easy

## Description
A lab technician tests the pH levels of unknown substances.

The pH meter records the pH level of $N$ samples in an array. To categorize acidity, the technician needs to assign a rank to every sample based on its pH level.

The ranking rules are simple: the sample with the **smallest** pH level gets **Rank 1**. The next distinct pH level gets **Rank 2**, and so on.

If two or more samples have the exact same pH level, they must receive the **same rank**. The ranks must be integers starting from 1.

Your task is to replace each sample's pH level with its corresponding rank.

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
All samples share the same pH level, so they share Rank 1.

## Input Format
- The first line contains an integer `n`, the number of samples.
- The second line contains `n` space-separated integers representing the pH levels.

## Output Format
- Return an array of integers where each element is the rank of the corresponding sample.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, sorting
