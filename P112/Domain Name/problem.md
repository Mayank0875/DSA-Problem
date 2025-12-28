## Title
Domain Name

## Slug
domain-name

## Difficulty
Easy

## Description
A squatter tracks the value of 'meta.com'. They want to buy the domain and sell it to a tech giant.

You have a list of domain price for $n$ consecutive months. You want to make one perfect move: register on one month and transfer on a different month in the future. You cannot transfer before you register.

Your goal is to find the **maximum possible payout** you can earn from this single transaction. If it is impossible to make any payout (i.e., the domain price only goes down), you should return 0.

## Examples

### 1

#### Input
6
7 1 5 3 6 4

#### Output
5

#### Explanation
register on month 2 (domain price = 1) and transfer on month 5 (domain price = 6). The payout is $6 - 1 = 5$.
Note that registering on month 1 (domain price = 7) is not optimal, as all future values are lower.

### 2

#### Input
5
7 6 4 3 1

#### Output
0

#### Explanation
The domain price never increases, so it is impossible to make a payout. The maximum payout is 0.

## Input Format
- The first line contains a single integer `n`, the number of months.
- The second line contains `n` space-separated integers representing the domain price on each month.

## Output Format
- Return a single integer representing the maximum payout. If no payout can be made, return 0.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ values ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy
