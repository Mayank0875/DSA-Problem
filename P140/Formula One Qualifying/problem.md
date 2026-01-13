## Title
Formula One Qualifying

## Slug
formula-one-qualifying

## Difficulty
Easy

## Description
Drivers are completing qualifying laps. The fastest times (lowest values) get the best starting positions.

The race computer records the lap time of $N$ cars in an array. To set the grid, the steward needs to assign a rank to every car based on its lap time.

The ranking rules are simple: the car with the **smallest** lap time gets **Rank 1**. The next distinct lap time gets **Rank 2**, and so on.

If two or more cars have the exact same lap time, they must receive the **same rank**. The ranks must be integers starting from 1.

Your task is to replace each car's lap time with its corresponding rank.

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
All cars share the same lap time, so they share Rank 1.

## Input Format
- The first line contains an integer `n`, the number of cars.
- The second line contains `n` space-separated integers representing the lap times.

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
