## Title
Apartment Hunting

## Slug
apartment-hunting

## Difficulty
Easy

## Description
A real estate agent lists apartments by monthly rent.

The listing service records the rent cost of $N$ apartments in an array. To help clients budget, the agent needs to assign a rank to every apartment based on its rent cost.

The ranking rules are simple: the apartment with the **smallest** rent cost gets **Rank 1**. The next distinct rent cost gets **Rank 2**, and so on.

If two or more apartments have the exact same rent cost, they must receive the **same rank**. The ranks must be integers starting from 1.

Your task is to replace each apartment's rent cost with its corresponding rank.

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
All apartments share the same rent cost, so they share Rank 1.

## Input Format
- The first line contains an integer `n`, the number of apartments.
- The second line contains `n` space-separated integers representing the rent costs.

## Output Format
- Return an array of integers where each element is the rank of the corresponding apartment.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, sorting
