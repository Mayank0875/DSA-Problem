## Title
Ticket to Mars

## Slug
ticket-to-mars

## Difficulty
Easy

## Description
SpaceX releases tickets. You want to buy a seat on the first shuttle and sell it to a billionaire.

You have a list of seat price for $n$ consecutive months. You want to make one perfect move: reserve on one month and auction on a different month in the future. You cannot auction before you reserve.

Your goal is to find the **maximum possible fortune** you can earn from this single transaction. If it is impossible to make any fortune (i.e., the seat price only goes down), you should return 0.

## Examples

### 1

#### Input
6
7 1 5 3 6 4

#### Output
5

#### Explanation
reserve on month 2 (seat price = 1) and auction on month 5 (seat price = 6). The fortune is $6 - 1 = 5$.
Note that reserveing on month 1 (seat price = 7) is not optimal, as all future values are lower.

### 2

#### Input
5
7 6 4 3 1

#### Output
0

#### Explanation
The seat price never increases, so it is impossible to make a fortune. The maximum fortune is 0.

## Input Format
- The first line contains a single integer `n`, the number of months.
- The second line contains `n` space-separated integers representing the seat price on each month.

## Output Format
- Return a single integer representing the maximum fortune. If no fortune can be made, return 0.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ values ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy
