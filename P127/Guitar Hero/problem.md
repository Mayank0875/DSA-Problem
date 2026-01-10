## Title
Guitar Hero

## Slug
guitar-hero

## Difficulty
Medium

## Description
A player hits notes. 1 is Hit, 0 is Miss. Star Power saves the combo multiplier for k misses.

You play a rhythm game represented by an array `nums` consisting of 1s (hits) and 0s (misses), and an integer `k`. You are allowed to save at most `k` missess from the sequence.

Your task is to find the length of the longest contiguous sequence of hitss after performing the saves. If the sequence contains no hitss even after optimal saves, return 0.

## Examples

### 1

#### Input
4
1 1 0 1
1

#### Output
3

#### Explanation
After saving the element at position 2 (value 0), the sequence becomes `[1, 1, 1]`. The longest segment of hitss has length 3.

### 2

#### Input
9
0 1 1 1 0 1 1 0 1
2

#### Output
6

#### Explanation
We can save the misses at index 4 and the misses at index 7. The resulting segments of hitss merge to form a sequence of length 6.

## Input Format
- The first line contains an integer `n`, representing the size of the array.
- The second line contains `n` space-separated integers representing the array `nums` (1 for hits, 0 for misses).
- The third line contains an integer `k`.

## Output Format
- Return a single integer representing the maximum size of the subarray of hitss.

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
