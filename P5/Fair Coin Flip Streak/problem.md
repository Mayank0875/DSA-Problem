## Title

Fair Coin Flip Streak

## Slug

fair-coin-flip-streak

## Difficulty

Easy

## Description

Imagine flipping a coin N times and recording the results, with '0' for tails and '1' for heads. We want to find the longest continuous sequence of flips within this record where the number of heads is exactly equal to the number of tails. This represents the longest "fair streak" in the sequence. Given the recorded coin flips, calculate the length of this longest fair streak.

## Examples

### 1

#### Input

2
[0, 1]

#### Output

2

#### Explanation

The streak [0, 1] (Tails, Heads) is the longest fair streak.

### 2

#### Input

3
[0, 1, 0]

#### Output

2

#### Explanation

[0, 1] (Tails, Heads) and [1, 0] (Heads, Tails) are the longest fair streaks.

## Input Format

- The first line contains a single integer N, the total number of coin flips.
- The second line contains N space-separated integers, representing the flip outcomes (0 for tails, 1 for heads).

## Output Format

- Return a single integer representing the length of the longest contiguous fair streak.

## Constraints

- 1 ≤ N ≤ 10^5
- 0 ≤ arr[i] ≤ 1

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, probability, prefix sum, hashmap