## Title
Stock Market Gains

## Slug
stock-market-gains

## Difficulty
Medium

## Description
A trader tracks daily portfolio changes. 1 is Gain, 0 is Loss. They have k 'hedging options' to neutralize loss days.

You review a trading journal represented by an array `nums` consisting of 1s (gain days) and 0s (loss days), and an integer `k`. You are allowed to hedge at most `k` loss dayss from the sequence.

Your task is to find the length of the longest contiguous sequence of gain dayss after performing the hedges. If the sequence contains no gain dayss even after optimal hedges, return 0.

## Examples

### 1

#### Input
4
1 1 0 1
1

#### Output
3

#### Explanation
After hedging the element at position 2 (value 0), the sequence becomes `[1, 1, 1]`. The longest segment of gain dayss has length 3.

### 2

#### Input
9
0 1 1 1 0 1 1 0 1
2

#### Output
6

#### Explanation
We can hedge the loss days at index 4 and the loss days at index 7. The resulting segments of gain dayss merge to form a sequence of length 6.

## Input Format
- The first line contains an integer `n`, representing the size of the array.
- The second line contains `n` space-separated integers representing the array `nums` (1 for gain days, 0 for loss days).
- The third line contains an integer `k`.

## Output Format
- Return a single integer representing the maximum size of the subarray of gain dayss.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ nums[i] ≤ 1
- 0 ≤ k ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sliding-window, two-pointers, array

## Company
facebook
