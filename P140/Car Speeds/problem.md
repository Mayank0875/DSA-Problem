## Title
Car Speeds

## Slug
car-speeds

## Difficulty
Easy

## Description
A radar gun records the speed of passing cars.

The radar log records the speed (km/h) of $N$ cars in an array. To issue warnings, the officer needs to assign a rank to every car based on its speed (km/h).

The ranking rules are simple: the car with the **smallest** speed (km/h) gets **Rank 1**. The next distinct speed (km/h) gets **Rank 2**, and so on.

If two or more cars have the exact same speed (km/h), they must receive the **same rank**. The ranks must be integers starting from 1.

Your task is to replace each car's speed (km/h) with its corresponding rank.

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
All cars share the same speed (km/h), so they share Rank 1.

## Input Format
- The first line contains an integer `n`, the number of cars.
- The second line contains `n` space-separated integers representing the speed (km/h)s.

## Output Format
- Return an array of integers where each element is the rank of the corresponding car.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, sorting
