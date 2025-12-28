## Title
Battery Range

## Slug
battery-range

## Difficulty
Medium

## Description
An electric car travels between charging stations. Each station provides enough charge to reach a certain distance forward.

You start at the **first charging station** (index 0). Each charging station has a specific charge capacity, given by an integer array `nums`. The value at `nums[i]` represents the **maximum length** you can drive forward from that position.

For example, if you are at index `i` and `nums[i] = 3`, you can drive to any charging station at index `i+1`, `i+2`, or `i+3`.

Your goal is to determine if it is possible to reach the **last charging station** (the final index of the array) starting from the first.

Return `true` if you can reach the last index, or `false` otherwise.

## Examples

### 1

#### Input
5
2 3 1 1 4

#### Output
true

#### Explanation
Drive 1 step from index 0 to 1, then drive 3 steps to the last index.

### 2

#### Input
5
3 2 1 0 4

#### Output
false

#### Explanation
You will always arrive at index 3 no matter what. Its maximum drive length is 0, which makes it impossible to advance further to the last index.

## Input Format
- The first line contains an integer `n`, the number of charging stations.
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
