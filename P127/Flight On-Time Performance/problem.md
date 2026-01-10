## Title
Flight On-Time Performance

## Slug
flight-on-time-performance

## Difficulty
Medium

## Description
An airline tracks arrivals. 1 is On Time, 0 is Late. They can attribute k late flights to 'weather' to exclude them from metrics.

You analyze flight logs represented by an array `nums` consisting of 1s (on-time flights) and 0s (late flights), and an integer `k`. You are allowed to exclude at most `k` late flightss from the sequence.

Your task is to find the length of the longest contiguous sequence of on-time flightss after performing the exclusions. If the sequence contains no on-time flightss even after optimal exclusions, return 0.

## Examples

### 1

#### Input
4
1 1 0 1
1

#### Output
3

#### Explanation
After excluding the element at position 2 (value 0), the sequence becomes `[1, 1, 1]`. The longest segment of on-time flightss has length 3.

### 2

#### Input
9
0 1 1 1 0 1 1 0 1
2

#### Output
6

#### Explanation
We can exclude the late flights at index 4 and the late flights at index 7. The resulting segments of on-time flightss merge to form a sequence of length 6.

## Input Format
- The first line contains an integer `n`, representing the size of the array.
- The second line contains `n` space-separated integers representing the array `nums` (1 for on-time flights, 0 for late flights).
- The third line contains an integer `k`.

## Output Format
- Return a single integer representing the maximum size of the subarray of on-time flightss.

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
