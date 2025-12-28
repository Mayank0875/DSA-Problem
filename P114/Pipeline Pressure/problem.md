## Title
Pipeline Pressure

## Slug
pipeline-pressure

## Difficulty
Medium

## Description
Gas flows in a pipe. Booster pumps increase pressure to push gas through segments.

You start at the **first segment** (index 0). Each segment has a specific pressure boost, given by an integer array `nums`. The value at `nums[i]` represents the **maximum length** you can push forward from that position.

For example, if you are at index `i` and `nums[i] = 3`, you can push to any segment at index `i+1`, `i+2`, or `i+3`.

Your goal is to determine if it is possible to reach the **last segment** (the final index of the array) starting from the first.

Return `true` if you can reach the last index, or `false` otherwise.

## Examples

### 1

#### Input
5
2 3 1 1 4

#### Output
true

#### Explanation
Push 1 step from index 0 to 1, then push 3 steps to the last index.

### 2

#### Input
5
3 2 1 0 4

#### Output
false

#### Explanation
You will always arrive at index 3 no matter what. Its maximum push length is 0, which makes it impossible to advance further to the last index.

## Input Format
- The first line contains an integer `n`, the number of segments.
- The second line contains `n` space-separated integers representing the `nums` array.

## Output Format
- Return `true` if the last index is reachable, `false` otherwise.

## Constraints
- 1 ≤ n ≤ 10^4
- 0 ≤ nums[i] ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy
