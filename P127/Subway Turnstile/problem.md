## Title
Subway Turnstile

## Slug
subway-turnstile

## Difficulty
Medium

## Description
Commuters pass through. 1 is Valid Ticket, 0 is Error. An attendant can manually open the gate for k errors.

You monitor turnstile logs represented by an array `nums` consisting of 1s (valid entries) and 0s (errors), and an integer `k`. You are allowed to override at most `k` errorss from the sequence.

Your task is to find the length of the longest contiguous sequence of valid entriess after performing the overrides. If the sequence contains no valid entriess even after optimal overrides, return 0.

## Examples

### 1

#### Input
4
1 1 0 1
1

#### Output
3

#### Explanation
After overriding the element at position 2 (value 0), the sequence becomes `[1, 1, 1]`. The longest segment of valid entriess has length 3.

### 2

#### Input
9
0 1 1 1 0 1 1 0 1
2

#### Output
6

#### Explanation
We can override the errors at index 4 and the errors at index 7. The resulting segments of valid entriess merge to form a sequence of length 6.

## Input Format
- The first line contains an integer `n`, representing the size of the array.
- The second line contains `n` space-separated integers representing the array `nums` (1 for valid entries, 0 for errors).
- The third line contains an integer `k`.

## Output Format
- Return a single integer representing the maximum size of the subarray of valid entriess.

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
