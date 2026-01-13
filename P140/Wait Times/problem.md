## Title
Wait Times

## Slug
wait-times

## Difficulty
Easy

## Description
A theme park app shows wait times for rides.

The app records the wait (mins) of $N$ rides in an array. To plan the day, the visitor needs to assign a rank to every ride based on its wait (mins).

The ranking rules are simple: the ride with the **smallest** wait (mins) gets **Rank 1**. The next distinct wait (mins) gets **Rank 2**, and so on.

If two or more rides have the exact same wait (mins), they must receive the **same rank**. The ranks must be integers starting from 1.

Your task is to replace each ride's wait (mins) with its corresponding rank.

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
All rides share the same wait (mins), so they share Rank 1.

## Input Format
- The first line contains an integer `n`, the number of rides.
- The second line contains `n` space-separated integers representing the wait (mins)s.

## Output Format
- Return an array of integers where each element is the rank of the corresponding ride.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, sorting
