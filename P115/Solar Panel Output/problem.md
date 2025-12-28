## Title
Solar Panel Output

## Slug
solar-panel-output

## Difficulty
Medium

## Description
As the sun rises, panel output increases. Passing clouds caused a chaotic dip in the readings.

A valid energy log must be optimal, meaning the wattage should appear in non-decreasing order.

However, clouds has inserted a chunk of incorrect wattage into the middle of the energy log, corrupting it. To fix this, you must remove a single contiguous sequence of wattage (a subarray) so that the remaining wattage form a sorted, non-decreasing sequence.

Your goal is to minimize the data ignored. Determine the length of the **shortest contiguous subarray** that needs to be removed to restore the non-decreasing order of the remaining wattage.

## Examples

### 1

#### Input
8
1 2 3 10 4 2 3 5

#### Output
3

#### Explanation
The shortest subarray to remove is `[10, 4, 2]` (indices 3, 4, 5). The remaining energy log is `[1, 2, 3, 3, 5]`, which is sorted. Removing `[3, 10, 4]` is also a valid solution of length 3.

### 2

#### Input
5
5 4 3 2 1

#### Output
4

#### Explanation
Since the energy log is strictly decreasing, we can only keep one wattage. We must remove a subarray of length 4 (e.g., `[5, 4, 3, 2]` leaving `[1]`).

## Input Format
- The first line contains an integer `n`, the number of wattage.
- The second line contains `n` space-separated integers representing the `watts` array.

## Output Format
- Return a single integer representing the length of the shortest subarray to remove.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ watts[i] ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, two-pointers, binary-search
