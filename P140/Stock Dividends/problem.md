## Title
Stock Dividends

## Slug
stock-dividends

## Difficulty
Easy

## Description
An investor ranks stocks by dividend yield.

The portfolio records the yield % of $N$ stocks in an array. To maximize returns, the investor needs to assign a rank to every stock based on its yield %.

The ranking rules are simple: the stock with the **smallest** yield % gets **Rank 1**. The next distinct yield % gets **Rank 2**, and so on.

If two or more stocks have the exact same yield %, they must receive the **same rank**. The ranks must be integers starting from 1.

Your task is to replace each stock's yield % with its corresponding rank.

## Examples

### 1

#### Input
4
40 10 20 30

#### Output
4 1 2 3

#### Explanation
10 is the smallest (Rank 1). 20 is the second smallest (Rank 2). 30 is third (Rank 3). 40 is largest (Rank 4).

### 2

#### Input
3
2 2 2

#### Output
1 1 1

#### Explanation
All stocks share the same yield %, so they share Rank 1.

## Input Format
- The first line contains an integer `n`, the number of stocks.
- The second line contains `n` space-separated integers representing the yield %s.

## Output Format
- Return an array of integers where each element is the rank of the corresponding stock.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, sorting
