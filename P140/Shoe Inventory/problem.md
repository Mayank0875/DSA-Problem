## Title
Shoe Inventory

## Slug
shoe-inventory

## Difficulty
Easy

## Description
A store clerk organizes shoes by size on the rack.

The inventory list records the size of $N$ shoes in an array. To tidy the display, the clerk needs to assign a rank to every shoe based on its size.

The ranking rules are simple: the shoe with the **smallest** size gets **Rank 1**. The next distinct size gets **Rank 2**, and so on.

If two or more shoes have the exact same size, they must receive the **same rank**. The ranks must be integers starting from 1.

Your task is to replace each shoe's size with its corresponding rank.

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
All shoes share the same size, so they share Rank 1.

## Input Format
- The first line contains an integer `n`, the number of shoes.
- The second line contains `n` space-separated integers representing the sizes.

## Output Format
- Return an array of integers where each element is the rank of the corresponding shoe.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, sorting
