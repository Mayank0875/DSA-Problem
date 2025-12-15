## Title
Factory Production Shifts

## Slug
factory-production-shifts

## Difficulty
Hard

## Description
A factory has `n` orders to process in `k` shifts. The orders have different difficulty ratings. Orders are processed sequentially. The 'worker strain' for a shift is the square of the sum of difficulty ratings completed in that shift.

You must partition the sequence of orders into exactly `k` non-empty contiguous shifts.
Each shift corresponds to a shift.
The "worker strain" for a shift is calculated as the **square of the sum** of the difficulty ratings of the orders in that shift.

Your goal is to minimize the total worker strain (the sum of the worker strain values of all `k` shifts).

## Examples

### 1

#### Input
8 3
2 3 1 2 2 3 4 1

#### Output
110

#### Explanation
We partition the orders into 3 shifts: `[2, 3, 1]`, `[2, 2, 3]`, and `[4, 1]`.
The sums are 6, 7, 5.
The total worker strain is $6^2 + 7^2 + 5^2 = 36 + 49 + 25 = 110$.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
225

#### Explanation
Only 1 shift is allowed, containing all orders. Sum = 15. worker strain = $15^2 = 225$.

## Input Format
- The first line contains two integers `n` and `k`: the number of orders and the required number of shifts.
- The second line contains `n` integers representing the difficulty ratings of each order.

## Output Format
- Return one integer: the minimum total worker strain.

## Constraints
- 1 ≤ k ≤ n ≤ 3000
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, array
