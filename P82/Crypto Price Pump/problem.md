## Title
Crypto Price Pump

## Slug
crypto-price-pump

## Difficulty
Easy

## Description
A trader looks at n hourly prices. They want to find the longest 'pump' sequence.

You have n hourly prices.
A pump sequence consists of hours where the price is strictly higher than the previous hour.

You must analyze the chart to find the longest possible pump sequence. You can skip any number of prices to form the sequence, but you must maintain the original time order of the selected prices. Calculate the maximum number of prices that can form such a sequence.

## Examples

### 1

#### Input
8
7 3 5 3 6 2 9 8

#### Output
4

#### Explanation
The input contains: [7, 3, 5, 3, 6, 2, 9, 8]. The longest pump sequences (strictly increasing) include:
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
- The second line contains n integers x_1, x_2 ... x_n: the value of each price in order.

## Output Format
- Return one integer: the length of the longest valid pump sequence.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, dynamic-programming, greedy
