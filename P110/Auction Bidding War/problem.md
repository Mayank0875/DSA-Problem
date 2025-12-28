## Title
Auction Bidding War

## Slug
auction-bidding-war

## Difficulty
Easy

## Description
An auctioneer reviews a log of bids. A 'Bidding War' is a sequence of consecutive bids where each bid is strictly higher than the last.

The Auctioneer is analyzing a sequence of bids represented by an array of integers `nums`, where `nums[i]` represents the dollar amount at index `i`.

The Auctioneer wants to find the maximum total dollar amount obtained during a single "**Bidding War**". A "Bidding War" is defined as a contiguous subarray of bids where the dollar amount of each bid is `strictly greater` than the previous one.

Your task is to find the **maximum sum** of dollar amounts possible from one such Bidding War. The Bidding War must include at least one bid.

## Examples

### 1

#### Input
6
10 20 30 5 10 50

#### Output
65

#### Explanation
The The Auctioneer identifies the sequence `[10, 20, 30]` with a sum of 60. However, a better Bidding War starts later: `[5, 10, 50]`. This is a strictly increasing contiguous subarray, and its sum is 65.

### 2

#### Input
5
10 20 30 40 50

#### Output
150

#### Explanation
The entire sequence is strictly increasing. The sum is 150.

## Input Format
- The first line contains a single integer `n`, the number of bids.
- The second line contains `n` space-separated integers, representing the dollar amounts.

## Output Format
- Return a single integer representing the maximum sum of any strictly increasing contiguous subarray.

## Constraints
- 1 ≤ n ≤ 100
- 1 ≤ nums[i] ≤ 100

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sliding-window, easy
