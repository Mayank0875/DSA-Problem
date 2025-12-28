## Title
Temperature Log

## Slug
temperature-log

## Difficulty
Medium

## Description
A scientist monitors a reaction that must strictly heat up. A sensor malfunction recorded a drop in temperature readings in the middle.

A valid temperature log must be stable, meaning the temperatures should appear in non-decreasing order.

However, a sensor error has inserted a chunk of incorrect temperatures into the middle of the temperature log, corrupting it. To fix this, you must remove a single contiguous sequence of temperatures (a subarray) so that the remaining temperatures form a sorted, non-decreasing sequence.

Your goal is to minimize the record gaps. Determine the length of the **shortest contiguous subarray** that needs to be removed to restore the non-decreasing order of the remaining temperatures.

## Examples

### 1

#### Input
8
1 2 3 10 4 2 3 5

#### Output
3

#### Explanation
The shortest subarray to remove is `[10, 4, 2]` (indices 3, 4, 5). The remaining temperature log is `[1, 2, 3, 3, 5]`, which is sorted. Removing `[3, 10, 4]` is also a valid solution of length 3.

### 2

#### Input
5
5 4 3 2 1

#### Output
4

#### Explanation
Since the temperature log is strictly decreasing, we can only keep one temperature. We must remove a subarray of length 4 (e.g., `[5, 4, 3, 2]` leaving `[1]`).

## Input Format
- The first line contains an integer `n`, the number of temperatures.
- The second line contains `n` space-separated integers representing the `temperatures` array.

## Output Format
- Return a single integer representing the length of the shortest subarray to remove.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ temperatures[i] ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, two-pointers, binary-search
