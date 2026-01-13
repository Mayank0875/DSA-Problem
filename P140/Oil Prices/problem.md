## Title
Oil Prices

## Slug
oil-prices

## Difficulty
Easy

## Description
A trader monitors crude oil prices from different regions.

The ticker records the price per barrel of $N$ regions in an array. To spot arbitrage, the trader needs to assign a rank to every region based on its price per barrel.

The ranking rules are simple: the region with the **smallest** price per barrel gets **Rank 1**. The next distinct price per barrel gets **Rank 2**, and so on.

If two or more regions have the exact same price per barrel, they must receive the **same rank**. The ranks must be integers starting from 1.

Your task is to replace each region's price per barrel with its corresponding rank.

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
All regions share the same price per barrel, so they share Rank 1.

## Input Format
- The first line contains an integer `n`, the number of regions.
- The second line contains `n` space-separated integers representing the price per barrels.

## Output Format
- Return an array of integers where each element is the rank of the corresponding region.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, sorting
