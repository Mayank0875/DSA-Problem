## Title
Auction Bids

## Slug
auction-bids

## Difficulty
Easy

## Description
An auctioneer reviews n bids. They want to trace the history of legitimate raises.

You have a list of n bids received.
A legitimate history consists of bids where the amount is strictly higher than the previous bid.

You must verify the history to find the longest possible bid chain. You can skip any number of bids to form the sequence, but you must maintain the original time order of the selected bids. Calculate the maximum number of bids that can form such a sequence.

## Examples

### 1

#### Input
8
7 3 5 3 6 2 9 8

#### Output
4

#### Explanation
The input contains: [7, 3, 5, 3, 6, 2, 9, 8]. The longest bid chains (strictly increasing) include:
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
Since the values are strictly decreasing, we can pick at most 1 bid.

## Input Format
- The first line contains an integer n: the number of bids.
- The second line contains n integers x_1, x_2 ... x_n: the amount of each bid in order.

## Output Format
- Return one integer: the length of the longest valid bid chain.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, dynamic-programming, greedy
