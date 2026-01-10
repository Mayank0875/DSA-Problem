## Title
Basketball Shooting

## Slug
basketball-shooting

## Difficulty
Medium

## Description
A player shoots hoops. 1 is a Basket, 0 is a Miss. In a highlight reel, the editor can cut up to k misses to make a streak.

You edit a video of shots represented by an array `nums` consisting of 1s (baskets) and 0s (misses), and an integer `k`. You are allowed to cut at most `k` missess from the sequence.

Your task is to find the length of the longest contiguous sequence of basketss after performing the cuts. If the sequence contains no basketss even after optimal cuts, return 0.

## Examples

### 1

#### Input
4
1 1 0 1
1

#### Output
3

#### Explanation
After cutting the element at position 2 (value 0), the sequence becomes `[1, 1, 1]`. The longest segment of basketss has length 3.

### 2

#### Input
9
0 1 1 1 0 1 1 0 1
2

#### Output
6

#### Explanation
We can cut the misses at index 4 and the misses at index 7. The resulting segments of basketss merge to form a sequence of length 6.

## Input Format
- The first line contains an integer `n`, representing the size of the array.
- The second line contains `n` space-separated integers representing the array `nums` (1 for baskets, 0 for misses).
- The third line contains an integer `k`.

## Output Format
- Return a single integer representing the maximum size of the subarray of basketss.

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
