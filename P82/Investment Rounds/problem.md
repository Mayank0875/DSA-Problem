## Title
Investment Rounds

## Slug
investment-rounds

## Difficulty
Easy

## Description
A startup has n funding offers. They want to accept a series of offers that strictly increase in valuation.

You have n funding offer valuations.
A funding series consists of offers where the valuation is strictly higher than the previous accepted offer.

You must accept offers to find the longest possible funding series. You can skip any number of offers to form the sequence, but you must maintain the original time received order of the selected offers. Calculate the maximum number of offers that can form such a sequence.

## Examples

### 1

#### Input
8
7 3 5 3 6 2 9 8

#### Output
4

#### Explanation
The input contains: [7, 3, 5, 3, 6, 2, 9, 8]. The longest funding seriess (strictly increasing) include:
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
Since the values are strictly decreasing, we can pick at most 1 offer.

## Input Format
- The first line contains an integer n: the number of offers.
- The second line contains n integers x_1, x_2 ... x_n: the valuation of each offer in order.

## Output Format
- Return one integer: the length of the longest valid funding series.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, dynamic-programming, greedy
