## Title
Auction Bidding

## Slug
auction-bidding

## Difficulty
Medium

## Description
In a reverse auction, the price drops. The auctioneer lowers the price by a value equal to a digit in the current price.

You start with a **price** of `n`. The goal is to reduce this price to exactly 0.

In one **price drop**, you can look at the digits of the current price, choose one **non-zero digit**, and subtract it from the current price.

For example, if the price is 27, the digits are 2 and 7. You can subtract 2 (getting 25) or 7 (getting 20).

Your task is to find the **minimum** number of price drops required to reduce the price to 0.

## Examples

### 1

#### Input
27

#### Output
5

#### Explanation
1. 27 - 7 = 20
2. 20 - 2 = 18
3. 18 - 8 = 10
4. 10 - 1 = 9
5. 9 - 9 = 0
Total price drops: 5.

### 2

#### Input
0

#### Output
0

#### Explanation
The price is already 0.

## Input Format
- The input contains a single integer `n`.

## Output Format
- Return a single integer representing the minimum number of price drops.

## Constraints
- 0 ≤ n ≤ 10^6

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, greedy, math, bfs
