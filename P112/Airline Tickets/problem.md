## Title
Airline Tickets

## Slug
airline-tickets

## Difficulty
Easy

## Description
You track the price of a flight to Tokyo. You want to buy the ticket and, hypothetically, sell it (if transferrable) when prices skyrocket.

You have a list of ticket price for $n$ consecutive days. You want to make one perfect move: book on one day and transfer on a different day in the future. You cannot transfer before you book.

Your goal is to find the **maximum possible savings** you can earn from this single transaction. If it is impossible to make any savings (i.e., the ticket price only goes down), you should return 0.

## Examples

### 1

#### Input
6
7 1 5 3 6 4

#### Output
5

#### Explanation
book on day 2 (ticket price = 1) and transfer on day 5 (ticket price = 6). The savings is $6 - 1 = 5$.
Note that booking on day 1 (ticket price = 7) is not optimal, as all future values are lower.

### 2

#### Input
5
7 6 4 3 1

#### Output
0

#### Explanation
The ticket price never increases, so it is impossible to make a savings. The maximum savings is 0.

## Input Format
- The first line contains a single integer `n`, the number of days.
- The second line contains `n` space-separated integers representing the ticket price on each day.

## Output Format
- Return a single integer representing the maximum savings. If no savings can be made, return 0.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ values ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy
