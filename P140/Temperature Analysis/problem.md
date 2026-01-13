## Title
Temperature Analysis

## Slug
temperature-analysis

## Difficulty
Easy

## Description
A meteorologist is ranking cities based on how cold they are.

The sensor network records the temperature of $N$ cities in an array. To identify cold fronts, the scientist needs to assign a rank to every city based on its temperature.

The ranking rules are simple: the city with the **smallest** temperature gets **Rank 1**. The next distinct temperature gets **Rank 2**, and so on.

If two or more cities have the exact same temperature, they must receive the **same rank**. The ranks must be integers starting from 1.

Your task is to replace each city's temperature with its corresponding rank.

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
All cities share the same temperature, so they share Rank 1.

## Input Format
- The first line contains an integer `n`, the number of cities.
- The second line contains `n` space-separated integers representing the temperatures.

## Output Format
- Return an array of integers where each element is the rank of the corresponding city.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, sorting
