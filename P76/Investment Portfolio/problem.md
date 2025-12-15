## Title
Investment Portfolio

## Slug
investment-portfolio

## Difficulty
Hard

## Description
An investor groups `n` assets into `k` distinct funds. Assets are listed by liquidity need and grouped contiguously by maturity date. The 'risk exposure' of a fund is the square of the total value of assets in it.

You must partition the sequence of assets into exactly `k` non-empty contiguous funds.
Each fund corresponds to a fund.
The "risk exposure" for a fund is calculated as the **square of the sum** of the values of the assets in that fund.

Your goal is to minimize the total risk exposure (the sum of the risk exposure values of all `k` funds).

## Examples

### 1

#### Input
8 3
2 3 1 2 2 3 4 1

#### Output
110

#### Explanation
We partition the assets into 3 funds: `[2, 3, 1]`, `[2, 2, 3]`, and `[4, 1]`.
The sums are 6, 7, 5.
The total risk exposure is $6^2 + 7^2 + 5^2 = 36 + 49 + 25 = 110$.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
225

#### Explanation
Only 1 fund is allowed, containing all assets. Sum = 15. risk exposure = $15^2 = 225$.

## Input Format
- The first line contains two integers `n` and `k`: the number of assets and the required number of funds.
- The second line contains `n` integers representing the values of each asset.

## Output Format
- Return one integer: the minimum total risk exposure.

## Constraints
- 1 ≤ k ≤ n ≤ 3000
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, array
