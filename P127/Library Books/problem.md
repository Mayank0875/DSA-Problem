## Title
Library Books

## Slug
library-books

## Difficulty
Medium

## Description
A librarian scans returns. 1 is On Time, 0 is Overdue. They can waive fines for k overdue books.

You scan returned books represented by an array `nums` consisting of 1s (on-time returns) and 0s (overdue returns), and an integer `k`. You are allowed to waive at most `k` overdue returnss from the sequence.

Your task is to find the length of the longest contiguous sequence of on-time returnss after performing the waivers. If the sequence contains no on-time returnss even after optimal waivers, return 0.

## Examples

### 1

#### Input
4
1 1 0 1
1

#### Output
3

#### Explanation
After waiving the element at position 2 (value 0), the sequence becomes `[1, 1, 1]`. The longest segment of on-time returnss has length 3.

### 2

#### Input
9
0 1 1 1 0 1 1 0 1
2

#### Output
6

#### Explanation
We can waive the overdue returns at index 4 and the overdue returns at index 7. The resulting segments of on-time returnss merge to form a sequence of length 6.

## Input Format
- The first line contains an integer `n`, representing the size of the array.
- The second line contains `n` space-separated integers representing the array `nums` (1 for on-time returns, 0 for overdue returns).
- The third line contains an integer `k`.

## Output Format
- Return a single integer representing the maximum size of the subarray of on-time returnss.

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
