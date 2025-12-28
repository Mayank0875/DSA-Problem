## Title
Concert Tickets

## Slug
concert-tickets

## Difficulty
Medium

## Description
Tickets are released in batches. Scalpers grab the front row, Fans (you) get the stalls, and Late Buyers get the nosebleeds.

There are $3n$ tickets of varying view quality available. The distribution follows a strict protocol. In each round, you must select any 3 tickets. The parties then claim them based on the following rules:

1. The **Scalpers** takes the ticket with the **maximum** view quality from the triplet.
2. You, the **Fans**, take the ticket with the **second maximum** view quality.
3. The **Late Buyers** takes the remaining ticket (the one with the minimum view quality).

This process repeats until all tickets are distributed. Your goal as the Fans is to maximize the total view quality of the tickets you acquire.

Given an array of integers `tickets`, where `tickets[i]` represents the view quality of the $i$-th ticket, return the maximum total view quality you can obtain.

## Examples

### 1

#### Input
6
2 4 1 2 7 8

#### Output
9

#### Explanation
You have 6 tickets. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. Scalpers takes `8`, you take `7`, Late Buyers takes `2`.
2. Pick the remaining `(1, 2, 4)`. Scalpers takes `4`, you take `2`, Late Buyers takes `1`.
Total view quality = $7 + 2 = 9$.

### 2

#### Input
3
2 4 5

#### Output
4

#### Explanation
There is only one triplet `(2, 4, 5)`. Scalpers takes `5`, you take `4`, Late Buyers takes `2`. Total = 4.

## Input Format
- The first line contains a single integer $3n$, the number of tickets.
- The second line contains $3n$ space-separated integers representing the `tickets` array.

## Output Format
- Return a single integer representing the maximum total view quality you can collect.

## Constraints
- 1 ≤ tickets.length ≤ 10^5
- `tickets.length` is divisible by 3.
- 1 ≤ tickets[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sorting, greedy, math
