## Title
Parking Meter

## Slug
parking-meter

## Difficulty
Medium

## Description
Meters are checked. 1 is Valid, 0 is Expired. The city allows k grace periods for expired meters.

You check parking meters represented by an array `nums` consisting of 1s (valid meters) and 0s (expired meters), and an integer `k`. You are allowed to grace at most `k` expired meterss from the sequence.

Your task is to find the length of the longest contiguous sequence of valid meterss after performing the grace periods. If the sequence contains no valid meterss even after optimal grace periods, return 0.

## Examples

### 1

#### Input
4
1 1 0 1
1

#### Output
3

#### Explanation
After gracing the element at position 2 (value 0), the sequence becomes `[1, 1, 1]`. The longest segment of valid meterss has length 3.

### 2

#### Input
9
0 1 1 1 0 1 1 0 1
2

#### Output
6

#### Explanation
We can grace the expired meters at index 4 and the expired meters at index 7. The resulting segments of valid meterss merge to form a sequence of length 6.

## Input Format
- The first line contains an integer `n`, representing the size of the array.
- The second line contains `n` space-separated integers representing the array `nums` (1 for valid meters, 0 for expired meters).
- The third line contains an integer `k`.

## Output Format
- Return a single integer representing the maximum size of the subarray of valid meterss.

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
