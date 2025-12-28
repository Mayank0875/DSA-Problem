## Title
Learning Curve

## Slug
learning-curve

## Difficulty
Easy

## Description
A student solves math problems. A 'Brain Storm' is a streak where the difficulty rating of each solved problem is strictly higher than the last.

The Student is analyzing a sequence of problems represented by an array of integers `nums`, where `nums[i]` represents the difficulty rating at index `i`.

The Student wants to find the maximum total difficulty rating obtained during a single "**Brain Storm**". A "Brain Storm" is defined as a contiguous subarray of problems where the difficulty rating of each problem is `strictly greater` than the previous one.

Your task is to find the **maximum sum** of difficulty ratings possible from one such Brain Storm. The Brain Storm must include at least one problem.

## Examples

### 1

#### Input
6
10 20 30 5 10 50

#### Output
65

#### Explanation
The The Student identifies the sequence `[10, 20, 30]` with a sum of 60. However, a better Brain Storm starts later: `[5, 10, 50]`. This is a strictly increasing contiguous subarray, and its sum is 65.

### 2

#### Input
5
10 20 30 40 50

#### Output
150

#### Explanation
The entire sequence is strictly increasing. The sum is 150.

## Input Format
- The first line contains a single integer `n`, the number of problems.
- The second line contains `n` space-separated integers, representing the difficulty ratings.

## Output Format
- Return a single integer representing the maximum sum of any strictly increasing contiguous subarray.

## Constraints
- 1 ≤ n ≤ 100
- 1 ≤ nums[i] ≤ 100

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sliding-window, easy
