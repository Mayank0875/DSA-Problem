## Title
Calorie Count

## Slug
calorie-count

## Difficulty
Easy

## Description
A dietician ranks meals by caloric content.

The menu records the calories of $N$ meals in an array. To plan a diet, the dietician needs to assign a rank to every meal based on its calories.

The ranking rules are simple: the meal with the **smallest** calories gets **Rank 1**. The next distinct calories gets **Rank 2**, and so on.

If two or more meals have the exact same calories, they must receive the **same rank**. The ranks must be integers starting from 1.

Your task is to replace each meal's calories with its corresponding rank.

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
All meals share the same calories, so they share Rank 1.

## Input Format
- The first line contains an integer `n`, the number of meals.
- The second line contains `n` space-separated integers representing the caloriess.

## Output Format
- Return an array of integers where each element is the rank of the corresponding meal.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, sorting
