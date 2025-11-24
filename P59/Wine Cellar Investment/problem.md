## Title
Wine Cellar Investment

## Slug
wine-cellar-investment

## Difficulty
Easy

## Description
A sommelier buys a case of vintage wine. The value changes as the wine ages. They want to buy at a specific year and sell at a later year. Given the yearly valuation, find the maximum appreciation.

## Examples

### 1

#### Input
6
7 1 5 3 6 4

#### Output
5

#### Explanation
Buy at 1 (index 1) and sell at 6 (index 4). Profit = 6 - 1 = 5.

### 2

#### Input
5
7 6 4 3 1

#### Output
0

#### Explanation
Prices are strictly decreasing. No profit can be made.

## Input Format
- The first line contains an integer n, the number of entries.
- The second line contains n space-separated integers representing the sequence of values.

## Output Format
- Return a single integer representing the maximum possible gain (or 0 if none).

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ values[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
greedy, dynamic-programming
