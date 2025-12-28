## Title
Fuel Efficiency

## Slug
fuel-efficiency

## Difficulty
Medium

## Description
As an engine warms up, efficiency improves. A bad sensor reported random MPG values.

A valid engine monitor must be efficient, meaning the MPG should appear in non-decreasing order.

However, a bad sensor has inserted a chunk of incorrect MPG into the middle of the engine monitor, corrupting it. To fix this, you must remove a single contiguous sequence of MPG (a subarray) so that the remaining MPG form a sorted, non-decreasing sequence.

Your goal is to minimize the data points cleaned. Determine the length of the **shortest contiguous subarray** that needs to be removed to restore the non-decreasing order of the remaining MPG.

## Examples

### 1

#### Input
8
1 2 3 10 4 2 3 5

#### Output
3

#### Explanation
The shortest subarray to remove is `[10, 4, 2]` (indices 3, 4, 5). The remaining engine monitor is `[1, 2, 3, 3, 5]`, which is sorted. Removing `[3, 10, 4]` is also a valid solution of length 3.

### 2

#### Input
5
5 4 3 2 1

#### Output
4

#### Explanation
Since the engine monitor is strictly decreasing, we can only keep one MPG. We must remove a subarray of length 4 (e.g., `[5, 4, 3, 2]` leaving `[1]`).

## Input Format
- The first line contains an integer `n`, the number of MPG.
- The second line contains `n` space-separated integers representing the `mpgs` array.

## Output Format
- Return a single integer representing the length of the shortest subarray to remove.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ mpgs[i] ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, two-pointers, binary-search
