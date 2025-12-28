## Title
Stock Market Trends

## Slug
stock-market-trends

## Difficulty
Medium

## Description
An analyst identifies growth trends. Each trend has a buy price and a sell price.

The chart shows list of trends, each defined by a buy price and an sell price, represented as a pair `[buy, sell]`.

To compound gains in a specific strategy, the sell price of the previous trade must be strictly less than the buy price of the next trade. Specifically, to transition from trend `[a, b]` to a subsequent trend `[c, d]`, the sell of the first trend must be **strictly less than** the buy of the second trend (i.e., `b < c`).

You can select trends in any order you like to form a valid portfolio strategy. Your goal is to determine the maximum number of trends that can be included in a single portfolio strategy.

## Examples

### 1

#### Input
3
1 2
2 3
3 4

#### Output
2

#### Explanation
The longest portfolio strategy is `[1, 2] -> [3, 4]`. You cannot include `[2, 3]` because `2` (end of first) is not strictly less than `2` (start of second).

### 2

#### Input
3
1 2
7 8
4 5

#### Output
3

#### Explanation
The trends can be reordered to form the portfolio strategy `[1, 2] -> [4, 5] -> [7, 8]`. All transitions satisfy `end < start`.

## Input Format
- The first line contains an integer `n`, the number of available trends.
- The next `n` lines each contain two integers, representing the `buy` and `sell` of an trend.

## Output Format
- Return a single integer representing the maximum length of the portfolio strategy.

## Constraints
- 1 ≤ n ≤ 1000
- -1000 ≤ buy < sell ≤ 1000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy, sorting
