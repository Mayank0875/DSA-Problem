## Title
Customer Support Tickets

## Slug
customer-support-tickets

## Difficulty
Hard

## Description
A queue has `n` tickets. `k` agents pick batches of tickets. Tickets are handled FIFO. The 'stress level' of an agent is the square of the total complexity of tickets in their batch.

You must partition the sequence of tickets into exactly `k` non-empty contiguous batches.
Each batch corresponds to a agent.
The "stress level" for a agent is calculated as the **square of the sum** of the complexities of the tickets in that batch.

Your goal is to minimize the total stress level (the sum of the stress level values of all `k` batches).

## Examples

### 1

#### Input
8 3
2 3 1 2 2 3 4 1

#### Output
110

#### Explanation
We partition the tickets into 3 batches: `[2, 3, 1]`, `[2, 2, 3]`, and `[4, 1]`.
The sums are 6, 7, 5.
The total stress level is $6^2 + 7^2 + 5^2 = 36 + 49 + 25 = 110$.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
225

#### Explanation
Only 1 batch is allowed, containing all tickets. Sum = 15. stress level = $15^2 = 225$.

## Input Format
- The first line contains two integers `n` and `k`: the number of tickets and the required number of batches.
- The second line contains `n` integers representing the complexities of each ticket.

## Output Format
- Return one integer: the minimum total stress level.

## Constraints
- 1 ≤ k ≤ n ≤ 3000
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, array
