## Title
Winning Streak

## Slug
winning-streak

## Difficulty
Medium

## Description
A gamer tracks their match history. 1 is a Win, 0 is a Loss. They have k 'loss forgiveness' tokens to remove losses from their record.

You have a match history represented by an array `nums` consisting of 1s (wins) and 0s (losses), and an integer `k`. You are allowed to forgive at most `k` lossess from the sequence.

Your task is to find the length of the longest contiguous sequence of winss after performing the tokens. If the sequence contains no winss even after optimal tokens, return 0.

## Examples

### 1

#### Input
4
1 1 0 1
1

#### Output
3

#### Explanation
After forgiving the element at position 2 (value 0), the sequence becomes `[1, 1, 1]`. The longest segment of winss has length 3.

### 2

#### Input
9
0 1 1 1 0 1 1 0 1
2

#### Output
6

#### Explanation
We can forgive the losses at index 4 and the losses at index 7. The resulting segments of winss merge to form a sequence of length 6.

## Input Format
- The first line contains an integer `n`, representing the size of the array.
- The second line contains `n` space-separated integers representing the array `nums` (1 for wins, 0 for losses).
- The third line contains an integer `k`.

## Output Format
- Return a single integer representing the maximum size of the subarray of winss.

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
