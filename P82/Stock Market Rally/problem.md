## Title
Stock Market Rally

## Slug
stock-market-rally

## Difficulty
Easy

## Description
An investor wants to highlight a 'Bull Market' trend in a historical stock chart. A bull trend is defined by a series of stock prices where each price is strictly higher than the previous one picked.

You are given a timeline of n daily stock prices.
A valid trend consists of days picked such that the price on each chosen day is strictly greater than the price on the previously chosen day.

You must filter the timeline to find the longest possible bull trend. You can skip any number of prices to form the sequence, but you must maintain the original chronological order of the selected prices. Calculate the maximum number of prices that can form such a sequence.

## Examples

### 1

#### Input
8
7 3 5 3 6 2 9 8

#### Output
4

#### Explanation
The input contains: [7, 3, 5, 3, 6, 2, 9, 8]. The longest bull trends (strictly increasing) include:
3, 5, 6, 9
3, 5, 6, 8
The length of these sequences is 4.

### 2

#### Input
5
5 4 3 2 1

#### Output
1

#### Explanation
Since the values are strictly decreasing, we can pick at most 1 price.

## Input Format
- The first line contains an integer n: the number of prices.
- The second line contains n integers x_1, x_2 ... x_n: the price of each price in order.

## Output Format
- Return one integer: the length of the longest valid bull trend.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, dynamic-programming, greedy
