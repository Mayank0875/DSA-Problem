## Title
Staircase Construction

## Slug
staircase-construction

## Difficulty
Medium

## Description
A builder has stone blocks of various heights. A staircase requires blocks of consecutive height values. They want to build the tallest possible staircase.

Given an unsorted array of integers `heights` representing the block heights, return the length of the longest consecutive sequence of blocks that can be stacked into a staircase.

You must write an algorithm that runs in $O(n)$ time.

## Examples

### 1

#### Input
6
100 4 200 1 3 2

#### Output
4

#### Explanation
The longest consecutive sequence is `[1, 2, 3, 4]`. Therefore its length is 4.

### 2

#### Input
10
0 3 7 2 5 8 4 6 0 1

#### Output
9

#### Explanation
The consecutive sequence is `[0, 1, 2, 3, 4, 5, 6, 7, 8]`. Note that duplicates are handled (ignored or treated as part of the set existence).

## Input Format
- The first line contains an integer `n`, the number of blocks.
- The second line contains `n` space-separated integers representing the `heights` array.

## Output Format
- Return a single integer representing the length of the longest consecutive sequence.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ heights[i] ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table
