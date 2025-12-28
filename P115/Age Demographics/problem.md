## Title
Age Demographics

## Slug
age-demographics

## Difficulty
Medium

## Description
A survey lists participants by age. The data entry should be sorted, but a batch of forms was inserted out of order.

A valid survey list must be sorted, meaning the ages should appear in non-decreasing order.

However, a clerical error has inserted a chunk of incorrect ages into the middle of the survey list, corrupting it. To fix this, you must remove a single contiguous sequence of ages (a subarray) so that the remaining ages form a sorted, non-decreasing sequence.

Your goal is to minimize the discarded forms. Determine the length of the **shortest contiguous subarray** that needs to be removed to restore the non-decreasing order of the remaining ages.

## Examples

### 1

#### Input
8
1 2 3 10 4 2 3 5

#### Output
3

#### Explanation
The shortest subarray to remove is `[10, 4, 2]` (indices 3, 4, 5). The remaining survey list is `[1, 2, 3, 3, 5]`, which is sorted. Removing `[3, 10, 4]` is also a valid solution of length 3.

### 2

#### Input
5
5 4 3 2 1

#### Output
4

#### Explanation
Since the survey list is strictly decreasing, we can only keep one age. We must remove a subarray of length 4 (e.g., `[5, 4, 3, 2]` leaving `[1]`).

## Input Format
- The first line contains an integer `n`, the number of ages.
- The second line contains `n` space-separated integers representing the `ages` array.

## Output Format
- Return a single integer representing the length of the shortest subarray to remove.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ ages[i] ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, two-pointers, binary-search
