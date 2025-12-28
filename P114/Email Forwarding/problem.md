## Title
Email Forwarding

## Slug
email-forwarding

## Difficulty
Medium

## Description
An email chain propagates. Each recipient forwards it to a number of people down the list.

You start at the **first recipient** (index 0). Each recipient has a specific contact reach, given by an integer array `nums`. The value at `nums[i]` represents the **maximum length** you can forward forward from that position.

For example, if you are at index `i` and `nums[i] = 3`, you can forward to any recipient at index `i+1`, `i+2`, or `i+3`.

Your goal is to determine if it is possible to reach the **last recipient** (the final index of the array) starting from the first.

Return `true` if you can reach the last index, or `false` otherwise.

## Examples

### 1

#### Input
5
2 3 1 1 4

#### Output
true

#### Explanation
Forward 1 step from index 0 to 1, then forward 3 steps to the last index.

### 2

#### Input
5
3 2 1 0 4

#### Output
false

#### Explanation
You will always arrive at index 3 no matter what. Its maximum forward length is 0, which makes it impossible to advance further to the last index.

## Input Format
- The first line contains an integer `n`, the number of recipients.
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
