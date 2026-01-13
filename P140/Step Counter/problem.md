## Title
Step Counter

## Slug
step-counter

## Difficulty
Easy

## Description
Friends compete to see who walked the most steps.

The leaderboard records the step count of $N$ friends in an array. To determine the winner, the group needs to assign a rank to every friend based on its step count.

The ranking rules are simple: the friend with the **smallest** step count gets **Rank 1**. The next distinct step count gets **Rank 2**, and so on.

If two or more friends have the exact same step count, they must receive the **same rank**. The ranks must be integers starting from 1.

Your task is to replace each friend's step count with its corresponding rank.

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
All friends share the same step count, so they share Rank 1.

## Input Format
- The first line contains an integer `n`, the number of friends.
- The second line contains `n` space-separated integers representing the step counts.

## Output Format
- Return an array of integers where each element is the rank of the corresponding friend.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, sorting
