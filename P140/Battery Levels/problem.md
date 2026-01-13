## Title
Battery Levels

## Slug
battery-levels

## Difficulty
Easy

## Description
A charging station displays the charge percentage of connected EVs.

The display records the charge percentage of $N$ vehicles in an array. To prioritize charging, the system needs to assign a rank to every vehicle based on its charge percentage.

The ranking rules are simple: the vehicle with the **smallest** charge percentage gets **Rank 1**. The next distinct charge percentage gets **Rank 2**, and so on.

If two or more vehicles have the exact same charge percentage, they must receive the **same rank**. The ranks must be integers starting from 1.

Your task is to replace each vehicle's charge percentage with its corresponding rank.

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
All vehicles share the same charge percentage, so they share Rank 1.

## Input Format
- The first line contains an integer `n`, the number of vehicles.
- The second line contains `n` space-separated integers representing the charge percentages.

## Output Format
- Return an array of integers where each element is the rank of the corresponding vehicle.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, sorting
