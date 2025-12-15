## Title
Bakery Dough Batching

## Slug
bakery-dough-batching

## Difficulty
Hard

## Description
A baker processes `n` orders for bread using `k` mixers. Orders require different amounts of flour. Orders are processed in sequence. The 'mixer wear' is the square of the total flour weight in a batch.

You must partition the sequence of orders into exactly `k` non-empty contiguous batches.
Each batch corresponds to a mixer.
The "mixer wear" for a mixer is calculated as the **square of the sum** of the flour amounts of the orders in that batch.

Your goal is to minimize the total mixer wear (the sum of the mixer wear values of all `k` batches).

## Examples

### 1

#### Input
8 3
2 3 1 2 2 3 4 1

#### Output
110

#### Explanation
We partition the orders into 3 batches: `[2, 3, 1]`, `[2, 2, 3]`, and `[4, 1]`.
The sums are 6, 7, 5.
The total mixer wear is $6^2 + 7^2 + 5^2 = 36 + 49 + 25 = 110$.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
225

#### Explanation
Only 1 batch is allowed, containing all orders. Sum = 15. mixer wear = $15^2 = 225$.

## Input Format
- The first line contains two integers `n` and `k`: the number of orders and the required number of batches.
- The second line contains `n` integers representing the flour amounts of each order.

## Output Format
- Return one integer: the minimum total mixer wear.

## Constraints
- 1 ≤ k ≤ n ≤ 3000
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, array
