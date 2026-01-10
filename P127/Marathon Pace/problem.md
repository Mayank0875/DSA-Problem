## Title
Marathon Pace

## Slug
marathon-pace

## Difficulty
Medium

## Description
A runner tracks km splits. 1 is On Pace, 0 is Slow. They can sprint to make up time for k slow kms.

You monitor runner splits represented by an array `nums` consisting of 1s (on-pace splits) and 0s (slow splits), and an integer `k`. You are allowed to recover at most `k` slow splitss from the sequence.

Your task is to find the length of the longest contiguous sequence of on-pace splitss after performing the recoveries. If the sequence contains no on-pace splitss even after optimal recoveries, return 0.

## Examples

### 1

#### Input
4
1 1 0 1
1

#### Output
3

#### Explanation
After recovering the element at position 2 (value 0), the sequence becomes `[1, 1, 1]`. The longest segment of on-pace splitss has length 3.

### 2

#### Input
9
0 1 1 1 0 1 1 0 1
2

#### Output
6

#### Explanation
We can recover the slow splits at index 4 and the slow splits at index 7. The resulting segments of on-pace splitss merge to form a sequence of length 6.

## Input Format
- The first line contains an integer `n`, representing the size of the array.
- The second line contains `n` space-separated integers representing the array `nums` (1 for on-pace splits, 0 for slow splits).
- The third line contains an integer `k`.

## Output Format
- Return a single integer representing the maximum size of the subarray of on-pace splitss.

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
