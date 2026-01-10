## Title
Server Request

## Slug
server-request

## Difficulty
Medium

## Description
A server handles requests. 1 is 200 OK, 0 is 500 Error. A load balancer can retry k failed requests.

You analyze access logs represented by an array `nums` consisting of 1s (successful requests) and 0s (errors), and an integer `k`. You are allowed to retry at most `k` errorss from the sequence.

Your task is to find the length of the longest contiguous sequence of successful requestss after performing the retries. If the sequence contains no successful requestss even after optimal retries, return 0.

## Examples

### 1

#### Input
4
1 1 0 1
1

#### Output
3

#### Explanation
After retrying the element at position 2 (value 0), the sequence becomes `[1, 1, 1]`. The longest segment of successful requestss has length 3.

### 2

#### Input
9
0 1 1 1 0 1 1 0 1
2

#### Output
6

#### Explanation
We can retry the errors at index 4 and the errors at index 7. The resulting segments of successful requestss merge to form a sequence of length 6.

## Input Format
- The first line contains an integer `n`, representing the size of the array.
- The second line contains `n` space-separated integers representing the array `nums` (1 for successful requests, 0 for errors).
- The third line contains an integer `k`.

## Output Format
- Return a single integer representing the maximum size of the subarray of successful requestss.

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
