## Title
Glider Flight

## Slug
glider-flight

## Difficulty
Medium

## Description
A glider pilot uses thermals. Strong thermals provide lift to glide over miles of terrain.

You start at the **first thermal** (index 0). Each thermal has a specific lift strength, given by an integer array `nums`. The value at `nums[i]` represents the **maximum length** you can glide forward from that position.

For example, if you are at index `i` and `nums[i] = 3`, you can glide to any thermal at index `i+1`, `i+2`, or `i+3`.

Your goal is to determine if it is possible to reach the **last thermal** (the final index of the array) starting from the first.

Return `true` if you can reach the last index, or `false` otherwise.

## Examples

### 1

#### Input
5
2 3 1 1 4

#### Output
true

#### Explanation
Glide 1 step from index 0 to 1, then glide 3 steps to the last index.

### 2

#### Input
5
3 2 1 0 4

#### Output
false

#### Explanation
You will always arrive at index 3 no matter what. Its maximum glide length is 0, which makes it impossible to advance further to the last index.

## Input Format
- The first line contains an integer `n`, the number of thermals.
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
