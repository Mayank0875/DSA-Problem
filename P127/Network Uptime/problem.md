## Title
Network Uptime

## Slug
network-uptime

## Difficulty
Medium

## Description
A server logs status every minute. 1 is Up, 0 is Down. Maintenance can patch k minutes of downtime to make the log appear continuous.

You review server logs represented by an array `nums` consisting of 1s (uptime minutes) and 0s (downtime minutes), and an integer `k`. You are allowed to patch at most `k` downtime minutess from the sequence.

Your task is to find the length of the longest contiguous sequence of uptime minutess after performing the patches. If the sequence contains no uptime minutess even after optimal patches, return 0.

## Examples

### 1

#### Input
4
1 1 0 1
1

#### Output
3

#### Explanation
After patching the element at position 2 (value 0), the sequence becomes `[1, 1, 1]`. The longest segment of uptime minutess has length 3.

### 2

#### Input
9
0 1 1 1 0 1 1 0 1
2

#### Output
6

#### Explanation
We can patch the downtime minutes at index 4 and the downtime minutes at index 7. The resulting segments of uptime minutess merge to form a sequence of length 6.

## Input Format
- The first line contains an integer `n`, representing the size of the array.
- The second line contains `n` space-separated integers representing the array `nums` (1 for uptime minutes, 0 for downtime minutes).
- The third line contains an integer `k`.

## Output Format
- Return a single integer representing the maximum size of the subarray of uptime minutess.

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
