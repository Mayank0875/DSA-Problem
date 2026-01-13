## Title
Marathon Runners

## Slug
marathon-runners

## Difficulty
Easy

## Description
Runners cross the finish line at different timestamps.

The timer records the finish time of $N$ runners in an array. To assign placements, the official needs to assign a rank to every runner based on its finish time.

The ranking rules are simple: the runner with the **smallest** finish time gets **Rank 1**. The next distinct finish time gets **Rank 2**, and so on.

If two or more runners have the exact same finish time, they must receive the **same rank**. The ranks must be integers starting from 1.

Your task is to replace each runner's finish time with its corresponding rank.

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
All runners share the same finish time, so they share Rank 1.

## Input Format
- The first line contains an integer `n`, the number of runners.
- The second line contains `n` space-separated integers representing the finish times.

## Output Format
- Return an array of integers where each element is the rank of the corresponding runner.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, sorting
