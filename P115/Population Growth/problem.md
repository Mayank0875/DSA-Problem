## Title
Population Growth

## Slug
population-growth

## Difficulty
Medium

## Description
A city's population has been growing steadily. A data entry error input random numbers for the 90s.

A valid census record must be consistent, meaning the populations should appear in non-decreasing order.

However, data entry error has inserted a chunk of incorrect populations into the middle of the census record, corrupting it. To fix this, you must remove a single contiguous sequence of populations (a subarray) so that the remaining populations form a sorted, non-decreasing sequence.

Your goal is to minimize the years corrected. Determine the length of the **shortest contiguous subarray** that needs to be removed to restore the non-decreasing order of the remaining populations.

## Examples

### 1

#### Input
8
1 2 3 10 4 2 3 5

#### Output
3

#### Explanation
The shortest subarray to remove is `[10, 4, 2]` (indices 3, 4, 5). The remaining census record is `[1, 2, 3, 3, 5]`, which is sorted. Removing `[3, 10, 4]` is also a valid solution of length 3.

### 2

#### Input
5
5 4 3 2 1

#### Output
4

#### Explanation
Since the census record is strictly decreasing, we can only keep one population. We must remove a subarray of length 4 (e.g., `[5, 4, 3, 2]` leaving `[1]`).

## Input Format
- The first line contains an integer `n`, the number of populations.
- The second line contains `n` space-separated integers representing the `populations` array.

## Output Format
- Return a single integer representing the length of the shortest subarray to remove.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ populations[i] ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, two-pointers, binary-search
