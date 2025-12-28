## Title
Tree Growth

## Slug
tree-growth

## Difficulty
Easy

## Description
A biologist measures tree height annually. A 'Growth Spurt' is a series of years where the tree grew strictly more than the previous year.

The Biologist is analyzing a sequence of years represented by an array of integers `nums`, where `nums[i]` represents the growth amount at index `i`.

The Biologist wants to find the maximum total growth amount obtained during a single "**Growth Spurt**". A "Growth Spurt" is defined as a contiguous subarray of years where the growth amount of each year is `strictly greater` than the previous one.

Your task is to find the **maximum sum** of growth amounts possible from one such Growth Spurt. The Growth Spurt must include at least one year.

## Examples

### 1

#### Input
6
10 20 30 5 10 50

#### Output
65

#### Explanation
The The Biologist identifies the sequence `[10, 20, 30]` with a sum of 60. However, a better Growth Spurt starts later: `[5, 10, 50]`. This is a strictly increasing contiguous subarray, and its sum is 65.

### 2

#### Input
5
10 20 30 40 50

#### Output
150

#### Explanation
The entire sequence is strictly increasing. The sum is 150.

## Input Format
- The first line contains a single integer `n`, the number of years.
- The second line contains `n` space-separated integers, representing the growth amounts.

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
