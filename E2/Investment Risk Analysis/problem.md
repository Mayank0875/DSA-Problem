## Title
Investment Risk Analysis

## Slug
investment-risk-analysis

## Difficulty
Easy

## Description
A financial analyst is constructing a portfolio bundle for a client. The client has a very specific risk tolerance, defined by a target variance value. The analyst has a list of stocks, each with a known standard deviation metric. In this simplified model, the total variance of a portfolio of three uncorrelated stocks is the sum of the squares of their individual standard deviations. The analyst needs to know if it is possible to pick exactly three stocks from the market list to match the client's risk profile perfectly.

Your task is to determine whether it is possible to choose three distinct stocks (at indices i < j < k) such that:

    dev_i^2 + dev_j^2 + dev_k^2 = total_variance

If it is possible, print YES; otherwise, print NO.

## Examples

### 1
#### Input
5
1 2 2 3 4
9

#### Output
YES

#### Explanation
1^2 + 2^2 + 2^2 = 1 + 4 + 4 = 9.

### 2
#### Input
4
3 3 3 3
20

#### Output
NO

#### Explanation
Every square is 9; any sum of three squares is 27 which is not 20.

## Input Format
- First line: integer n — the number of stocks.
- Second line: n space-separated integers a1 a2 ... an — the deviation metrics (can be negative, zero, or positive).
- Third line: integer target — the target sum.

## Output Format
- Return true (YES) if there exist indices i < j < k with a[i]^2 + a[j]^2 + a[k]^2 = target, otherwise return false (NO).

## Constraints
- 3 ≤ n ≤ 2000
- -10^6 ≤ ai ≤ 10^6
- 0 ≤ target ≤ 3×10^12

## Time Limit
1 second

## Memory Limit
256 MB

## Tags 
two-pointers, sorting, array, maths
