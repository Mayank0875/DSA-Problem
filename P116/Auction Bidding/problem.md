## Title
Auction Bidding

## Slug
auction-bidding

## Difficulty
Medium

## Description
Bidders place range bids. Each bid has a min price and max price.

The ledger has list of bids, each defined by a min and an max, represented as a pair `[min, max]`.

To accept multiple non-overlapping bids, the max price of one bid must be strictly less than the min price of the next. Specifically, to transition from bid `[a, b]` to a subsequent bid `[c, d]`, the max of the first bid must be **strictly less than** the min of the second bid (i.e., `b < c`).

You can select bids in any order you like to form a valid winning set. Your goal is to determine the maximum number of bids that can be included in a single winning set.

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
The longest winning set is `[1, 2] -> [3, 4]`. You cannot include `[2, 3]` because `2` (end of first) is not strictly less than `2` (start of second).

### 2

#### Input
3
1 2
7 8
4 5

#### Output
3

#### Explanation
The bids can be reordered to form the winning set `[1, 2] -> [4, 5] -> [7, 8]`. All transitions satisfy `end < start`.

## Input Format
- The first line contains an integer `n`, the number of available bids.
- The next `n` lines each contain two integers, representing the `min` and `max` of an bid.

## Output Format
- Return a single integer representing the maximum length of the winning set.

## Constraints
- 1 ≤ n ≤ 1000
- -1000 ≤ min < max ≤ 1000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy, sorting
