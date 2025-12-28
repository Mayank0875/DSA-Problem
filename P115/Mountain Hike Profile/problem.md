## Title
Mountain Hike Profile

## Slug
mountain-hike-profile

## Difficulty
Medium

## Description
A climber plans a route that should always go uphill (or flat). A mapping error inserted a valley section into the elevation data.

A valid route profile must be monotonic, meaning the elevations should appear in non-decreasing order.

However, a GPS glitch has inserted a chunk of incorrect elevations into the middle of the route profile, corrupting it. To fix this, you must remove a single contiguous sequence of elevations (a subarray) so that the remaining elevations form a sorted, non-decreasing sequence.

Your goal is to minimize the path deviation. Determine the length of the **shortest contiguous subarray** that needs to be removed to restore the non-decreasing order of the remaining elevations.

## Examples

### 1

#### Input
8
1 2 3 10 4 2 3 5

#### Output
3

#### Explanation
The shortest subarray to remove is `[10, 4, 2]` (indices 3, 4, 5). The remaining route profile is `[1, 2, 3, 3, 5]`, which is sorted. Removing `[3, 10, 4]` is also a valid solution of length 3.

### 2

#### Input
5
5 4 3 2 1

#### Output
4

#### Explanation
Since the route profile is strictly decreasing, we can only keep one elevation. We must remove a subarray of length 4 (e.g., `[5, 4, 3, 2]` leaving `[1]`).

## Input Format
- The first line contains an integer `n`, the number of elevations.
- The second line contains `n` space-separated integers representing the `elevations` array.

## Output Format
- Return a single integer representing the length of the shortest subarray to remove.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ elevations[i] ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, two-pointers, binary-search
