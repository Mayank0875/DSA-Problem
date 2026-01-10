## Title
Sunny Vacation

## Slug
sunny-vacation

## Difficulty
Medium

## Description
A tourist checks the weather forecast for upcoming days. 1 represents a Sunny day, 0 represents Rain. They have k 'indoor activity vouchers' to essentially ignore rainy days.

You have a weather forecast represented by an array `nums` consisting of 1s (sunny days) and 0s (rainy days), and an integer `k`. You are allowed to skip at most `k` rainy dayss from the sequence.

Your task is to find the length of the longest contiguous sequence of sunny dayss after performing the skips. If the sequence contains no sunny dayss even after optimal skips, return 0.

## Examples

### 1

#### Input
4
1 1 0 1
1

#### Output
3

#### Explanation
After skipping the element at position 2 (value 0), the sequence becomes `[1, 1, 1]`. The longest segment of sunny dayss has length 3.

### 2

#### Input
9
0 1 1 1 0 1 1 0 1
2

#### Output
6

#### Explanation
We can skip the rainy days at index 4 and the rainy days at index 7. The resulting segments of sunny dayss merge to form a sequence of length 6.

## Input Format
- The first line contains an integer `n`, representing the size of the array.
- The second line contains `n` space-separated integers representing the array `nums` (1 for sunny days, 0 for rainy days).
- The third line contains an integer `k`.

## Output Format
- Return a single integer representing the maximum size of the subarray of sunny dayss.

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
