## Title
Security Guard Patrol

## Slug
security-guard-patrol

## Difficulty
Medium

## Description
A guard checks checkpoints. 1 is Secure, 0 is Breach. The guard can secure k breaches immediately.

You review patrol logs represented by an array `nums` consisting of 1s (secure points) and 0s (breaches), and an integer `k`. You are allowed to secure at most `k` breachess from the sequence.

Your task is to find the length of the longest contiguous sequence of secure pointss after performing the actions. If the sequence contains no secure pointss even after optimal actions, return 0.

## Examples

### 1

#### Input
4
1 1 0 1
1

#### Output
3

#### Explanation
After securing the element at position 2 (value 0), the sequence becomes `[1, 1, 1]`. The longest segment of secure pointss has length 3.

### 2

#### Input
9
0 1 1 1 0 1 1 0 1
2

#### Output
6

#### Explanation
We can secure the breaches at index 4 and the breaches at index 7. The resulting segments of secure pointss merge to form a sequence of length 6.

## Input Format
- The first line contains an integer `n`, representing the size of the array.
- The second line contains `n` space-separated integers representing the array `nums` (1 for secure points, 0 for breaches).
- The third line contains an integer `k`.

## Output Format
- Return a single integer representing the maximum size of the subarray of secure pointss.

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
