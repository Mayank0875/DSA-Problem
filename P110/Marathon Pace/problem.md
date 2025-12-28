## Title
Marathon Pace

## Slug
marathon-pace

## Difficulty
Easy

## Description
A runner negatively splits. A 'Kick' is a sequence of miles where their speed strictly increases.

The Runner is analyzing a sequence of miles represented by an array of integers `nums`, where `nums[i]` represents the speed at index `i`.

The Runner wants to find the maximum total speed obtained during a single "**Kick**". A "Kick" is defined as a contiguous subarray of miles where the speed of each mile is `strictly greater` than the previous one.

Your task is to find the **maximum sum** of speeds possible from one such Kick. The Kick must include at least one mile.

## Examples

### 1

#### Input
6
10 20 30 5 10 50

#### Output
65

#### Explanation
The The Runner identifies the sequence `[10, 20, 30]` with a sum of 60. However, a better Kick starts later: `[5, 10, 50]`. This is a strictly increasing contiguous subarray, and its sum is 65.

### 2

#### Input
5
10 20 30 40 50

#### Output
150

#### Explanation
The entire sequence is strictly increasing. The sum is 150.

## Input Format
- The first line contains a single integer `n`, the number of miles.
- The second line contains `n` space-separated integers, representing the speeds.

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
