## Title
Supermarket Checkout

## Slug
supermarket-checkout

## Difficulty
Hard

## Description
A conveyor belt has `n` items. The cashier bags them into `k` bags. Items are bagged in order. The 'tear risk' of a bag is the square of the total weight of items inside.

You must partition the sequence of items into exactly `k` non-empty contiguous bags.
Each bag corresponds to a bag.
The "tear risk" for a bag is calculated as the **square of the sum** of the weights of the items in that bag.

Your goal is to minimize the total tear risk (the sum of the tear risk values of all `k` bags).

## Examples

### 1

#### Input
8 3
2 3 1 2 2 3 4 1

#### Output
110

#### Explanation
We partition the items into 3 bags: `[2, 3, 1]`, `[2, 2, 3]`, and `[4, 1]`.
The sums are 6, 7, 5.
The total tear risk is $6^2 + 7^2 + 5^2 = 36 + 49 + 25 = 110$.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
225

#### Explanation
Only 1 bag is allowed, containing all items. Sum = 15. tear risk = $15^2 = 225$.

## Input Format
- The first line contains two integers `n` and `k`: the number of items and the required number of bags.
- The second line contains `n` integers representing the weights of each item.

## Output Format
- Return one integer: the minimum total tear risk.

## Constraints
- 1 ≤ k ≤ n ≤ 3000
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, array
