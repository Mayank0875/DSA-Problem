## Title
Ticket Prices

## Slug
ticket-prices

## Difficulty
Easy

## Description
A concert goer looks for seats by price tier.

The box office records the price of $N$ seats in an array. To buy a ticket, the fan needs to assign a rank to every seat based on its price.

The ranking rules are simple: the seat with the **smallest** price gets **Rank 1**. The next distinct price gets **Rank 2**, and so on.

If two or more seats have the exact same price, they must receive the **same rank**. The ranks must be integers starting from 1.

Your task is to replace each seat's price with its corresponding rank.

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
All seats share the same price, so they share Rank 1.

## Input Format
- The first line contains an integer `n`, the number of seats.
- The second line contains `n` space-separated integers representing the prices.

## Output Format
- Return an array of integers where each element is the rank of the corresponding seat.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, sorting
