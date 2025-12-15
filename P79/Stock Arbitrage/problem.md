## Title
Stock Arbitrage

## Slug
stock-arbitrage

## Difficulty
Medium

## Description
Traders exploit price differences. The market corrects the price gap after one trade.

The market consists of $n$ exchanges and $m$ one-way trades. Each trade connects a specific source exchange to a destination exchange.

The process happens over several orders. In each order, you must send a order from exchange 1 (the source) to exchange $n$ (the destination). The catch is that each trade vanishes as the market price corrects itself. This means each trade can be used at most once across all orders combined.

Your goal is to determine the maximum number of orders you can successfully complete the journey from exchange 1 to exchange $n$.

## Examples

### 1

#### Input
6 7
1 2
1 3
2 6
3 4
3 5
4 6
5 6

#### Output
2

#### Explanation
You can complete 2 orders.
Path 1: 1 -> 2 -> 6
Path 2: 1 -> 3 -> 4 -> 6 (or 1 -> 3 -> 5 -> 6)

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
You can complete 1 order.

## Input Format
- The first line contains two integers $n$ and $m$: the number of exchanges and the number of trades.
- The next $m$ lines describe the trades. Each line contains two integers $a$ and $b$, indicating a directed trade from exchange $a$ to exchange $b$.

## Output Format
- Return one integer: the maximum number of orders possible.

## Constraints
- 1 ≤ n ≤ 500
- 1 ≤ m ≤ 1000
- 1 ≤ a, b ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, breadth-first-search
