## Title
Web Page Load

## Slug
web-page-load

## Difficulty
Medium

## Description
A browser loads resources. 1 is Success, 0 is Timeout. The browser can retry k timed-out resources.

You load a web page represented by an array `nums` consisting of 1s (loaded resources) and 0s (timeouts), and an integer `k`. You are allowed to retry at most `k` timeoutss from the sequence.

Your task is to find the length of the longest contiguous sequence of loaded resourcess after performing the retries. If the sequence contains no loaded resourcess even after optimal retries, return 0.

## Examples

### 1

#### Input
4
1 1 0 1
1

#### Output
3

#### Explanation
After retrying the element at position 2 (value 0), the sequence becomes `[1, 1, 1]`. The longest segment of loaded resourcess has length 3.

### 2

#### Input
9
0 1 1 1 0 1 1 0 1
2

#### Output
6

#### Explanation
We can retry the timeouts at index 4 and the timeouts at index 7. The resulting segments of loaded resourcess merge to form a sequence of length 6.

## Input Format
- The first line contains an integer `n`, representing the size of the array.
- The second line contains `n` space-separated integers representing the array `nums` (1 for loaded resources, 0 for timeouts).
- The third line contains an integer `k`.

## Output Format
- Return a single integer representing the maximum size of the subarray of loaded resourcess.

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
