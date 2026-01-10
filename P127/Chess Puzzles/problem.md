## Title
Chess Puzzles

## Slug
chess-puzzles

## Difficulty
Medium

## Description
A player solves puzzles. 1 is Solved, 0 is Failed. They can use k hints to solve failed puzzles.

You solve daily puzzles represented by an array `nums` consisting of 1s (solved puzzles) and 0s (failed puzzles), and an integer `k`. You are allowed to hint at most `k` failed puzzless from the sequence.

Your task is to find the length of the longest contiguous sequence of solved puzzless after performing the hints. If the sequence contains no solved puzzless even after optimal hints, return 0.

## Examples

### 1

#### Input
4
1 1 0 1
1

#### Output
3

#### Explanation
After hinting the element at position 2 (value 0), the sequence becomes `[1, 1, 1]`. The longest segment of solved puzzless has length 3.

### 2

#### Input
9
0 1 1 1 0 1 1 0 1
2

#### Output
6

#### Explanation
We can hint the failed puzzles at index 4 and the failed puzzles at index 7. The resulting segments of solved puzzless merge to form a sequence of length 6.

## Input Format
- The first line contains an integer `n`, representing the size of the array.
- The second line contains `n` space-separated integers representing the array `nums` (1 for solved puzzles, 0 for failed puzzles).
- The third line contains an integer `k`.

## Output Format
- Return a single integer representing the maximum size of the subarray of solved puzzless.

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
