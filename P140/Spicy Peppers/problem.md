## Title
Spicy Peppers

## Slug
spicy-peppers

## Difficulty
Easy

## Description
A chili contest ranks peppers by Scoville heat units.

The lab report records the Scoville rating of $N$ peppers in an array. To warn contestants, the judge needs to assign a rank to every pepper based on its Scoville rating.

The ranking rules are simple: the pepper with the **smallest** Scoville rating gets **Rank 1**. The next distinct Scoville rating gets **Rank 2**, and so on.

If two or more peppers have the exact same Scoville rating, they must receive the **same rank**. The ranks must be integers starting from 1.

Your task is to replace each pepper's Scoville rating with its corresponding rank.

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
All peppers share the same Scoville rating, so they share Rank 1.

## Input Format
- The first line contains an integer `n`, the number of peppers.
- The second line contains `n` space-separated integers representing the Scoville ratings.

## Output Format
- Return an array of integers where each element is the rank of the corresponding pepper.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, sorting
