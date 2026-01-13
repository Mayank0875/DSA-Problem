## Title
Coin Values

## Slug
coin-values

## Difficulty
Easy

## Description
A collector sorts rare coins by their face value.

The collection records the face value of $N$ coins in an array. To catalog the set, the collector needs to assign a rank to every coin based on its face value.

The ranking rules are simple: the coin with the **smallest** face value gets **Rank 1**. The next distinct face value gets **Rank 2**, and so on.

If two or more coins have the exact same face value, they must receive the **same rank**. The ranks must be integers starting from 1.

Your task is to replace each coin's face value with its corresponding rank.

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
All coins share the same face value, so they share Rank 1.

## Input Format
- The first line contains an integer `n`, the number of coins.
- The second line contains `n` space-separated integers representing the face values.

## Output Format
- Return an array of integers where each element is the rank of the corresponding coin.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, sorting
