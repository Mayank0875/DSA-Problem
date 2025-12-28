## Title
IPO Launch

## Slug
ipo-launch

## Difficulty
Easy

## Description
An investor watches a new tech stock post-IPO. They want to buy shares and sell them during the initial hype.

You have a list of share price for $n$ consecutive minutes. You want to make one perfect move: buy in on one minute and cash out on a different minute in the future. You cannot cash out before you buy in.

Your goal is to find the **maximum possible capital gain** you can earn from this single transaction. If it is impossible to make any capital gain (i.e., the share price only goes down), you should return 0.

## Examples

### 1

#### Input
6
7 1 5 3 6 4

#### Output
5

#### Explanation
buy in on minute 2 (share price = 1) and cash out on minute 5 (share price = 6). The capital gain is $6 - 1 = 5$.
Note that buy ining on minute 1 (share price = 7) is not optimal, as all future values are lower.

### 2

#### Input
5
7 6 4 3 1

#### Output
0

#### Explanation
The share price never increases, so it is impossible to make a capital gain. The maximum capital gain is 0.

## Input Format
- The first line contains a single integer `n`, the number of minutes.
- The second line contains `n` space-separated integers representing the share price on each minute.

## Output Format
- Return a single integer representing the maximum capital gain. If no capital gain can be made, return 0.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ values ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy
