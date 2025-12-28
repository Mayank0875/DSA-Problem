## Title
Building Floors

## Slug
building-floors

## Difficulty
Medium

## Description
Floor numbers rise as you go up. A confusing hotel numbering system inserted random floors.

A valid elevator panel must be logical, meaning the floors should appear in non-decreasing order.

However, bad design has inserted a chunk of incorrect floors into the middle of the elevator panel, corrupting it. To fix this, you must remove a single contiguous sequence of floors (a subarray) so that the remaining floors form a sorted, non-decreasing sequence.

Your goal is to minimize the buttons removed. Determine the length of the **shortest contiguous subarray** that needs to be removed to restore the non-decreasing order of the remaining floors.

## Examples

### 1

#### Input
8
1 2 3 10 4 2 3 5

#### Output
3

#### Explanation
The shortest subarray to remove is `[10, 4, 2]` (indices 3, 4, 5). The remaining elevator panel is `[1, 2, 3, 3, 5]`, which is sorted. Removing `[3, 10, 4]` is also a valid solution of length 3.

### 2

#### Input
5
5 4 3 2 1

#### Output
4

#### Explanation
Since the elevator panel is strictly decreasing, we can only keep one floor. We must remove a subarray of length 4 (e.g., `[5, 4, 3, 2]` leaving `[1]`).

## Input Format
- The first line contains an integer `n`, the number of floors.
- The second line contains `n` space-separated integers representing the `floors` array.

## Output Format
- Return a single integer representing the length of the shortest subarray to remove.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ floors[i] ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, two-pointers, binary-search
