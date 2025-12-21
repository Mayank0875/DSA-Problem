## Title
Crypto Trading

## Slug
crypto-trading

## Difficulty
Hard

## Description
A bot executes trades. A strategy is 'profitable' if the total volume matches the missing order type.

TradeBot is analyzing a sequence of n trades. Each trade has a specific volume (a non-negative integer).

A contiguous group of trades is considered **profitable** if the sum of their volume values is exactly equal to the **Hidden Order** of that group.

The Hidden Order (Minimum Excluded Value or MEX) is defined as the smallest non-negative integer that does not exist among the volume values in the group.
For example:
- MEX of [1, 2] is 0
- MEX of [0, 2] is 1
- MEX of [0, 1, 2] is 3

Your task is to count the number of non-empty continuous subsegments that are profitable.

## Examples

### 1

#### Input
5
0 1 2 0 1

#### Output
4

#### Explanation
The profitable subsegments are:
- `[0, 1, 2]` (Indices 0-2): Sum = 3, MEX = 3.
- `[1, 2, 0]` (Indices 1-3): Sum = 3, MEX = 3.
- `[2, 0, 1]` (Indices 2-4): Sum = 3, MEX = 3.
- `[0, 1, 2, 0]` (Indices 0-3): Sum = 3, MEX = 3.

### 2

#### Input
3
1 1 1

#### Output
0

#### Explanation
No subsegment satisfies the condition. For `[1]`, Sum=1, MEX=0.

## Input Format
- The first line contains a single integer $n$ — the number of trades.
- The second line contains $n$ space-separated integers representing the volume values.

## Output Format
- Return a single integer representing the number of profitable subsegments.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ volume ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
two-pointers, maths, array
