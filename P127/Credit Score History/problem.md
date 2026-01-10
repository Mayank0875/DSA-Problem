## Title
Credit Score History

## Slug
credit-score-history

## Difficulty
Medium

## Description
A bank reviews payments. 1 is Paid, 0 is Missed. They allow k missed payments to be forgiven for long-term clients.

You review payment history represented by an array `nums` consisting of 1s (payments made) and 0s (missed payments), and an integer `k`. You are allowed to forgive at most `k` missed paymentss from the sequence.

Your task is to find the length of the longest contiguous sequence of payments mades after performing the waivers. If the sequence contains no payments mades even after optimal waivers, return 0.

## Examples

### 1

#### Input
4
1 1 0 1
1

#### Output
3

#### Explanation
After forgiving the element at position 2 (value 0), the sequence becomes `[1, 1, 1]`. The longest segment of payments mades has length 3.

### 2

#### Input
9
0 1 1 1 0 1 1 0 1
2

#### Output
6

#### Explanation
We can forgive the missed payments at index 4 and the missed payments at index 7. The resulting segments of payments mades merge to form a sequence of length 6.

## Input Format
- The first line contains an integer `n`, representing the size of the array.
- The second line contains `n` space-separated integers representing the array `nums` (1 for payments made, 0 for missed payments).
- The third line contains an integer `k`.

## Output Format
- Return a single integer representing the maximum size of the subarray of payments mades.

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
