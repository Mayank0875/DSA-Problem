## Title
Auction Bidding Window

## Slug
auction-bidding-window

## Difficulty
Easy

## Description
An online auction site tracks active bidder sessions.

The session log records the login and logout of every bidder in two integer arrays, `startTime` and `endTime`. The $i$-th bidder enters the auction at `startTime[i]` and leaves at `endTime[i]`, inclusive.

The auctioneer wants to know how many bidders were active during a specific final countdown `[queryStart, queryEnd]`. A bidder is considered active if their session overlaps with the final countdown at any point (even for a single moment).

Your task is to return the total number of bidders who were active during the given final countdown.

## Examples

### 1

#### Input
3
1 2 3
3 2 7
2 4

#### Output
3

#### Explanation
The final countdown is `[2, 4]`.
- Bidder 1 `[1, 3]` overlaps with `[2, 4]` (times 2, 3).
- Bidder 2 `[2, 2]` overlaps with `[2, 4]` (time 2).
- Bidder 3 `[3, 7]` overlaps with `[2, 4]` (times 3, 4).
All 3 bidders were active.

### 2

#### Input
1
4
4
1 3

#### Output
0

#### Explanation
The bidder was active at time `[4, 4]`. The final countdown is `[1, 3]`. There is no overlap.

## Input Format
- The first line contains an integer `n`, the number of bidders.
- The second line contains `n` space-separated integers for `startTime`.
- The third line contains `n` space-separated integers for `endTime`.
- The fourth line contains two integers, `queryStart` and `queryEnd`.

## Output Format
- Return a single integer representing the number of bidders active during the final countdown.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ startTime[i] ≤ endTime[i] ≤ 10^9
- 1 ≤ queryStart ≤ queryEnd ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, interval, linear-scan

## Company
amazon
