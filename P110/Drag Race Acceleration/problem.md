## Title
Drag Race Acceleration

## Slug
drag-race-acceleration

## Difficulty
Easy

## Description
A drag racer analyzes their speed trap data. A 'Perfect Launch' is a series of checkpoints where speed strictly increases.

The Racer is analyzing a sequence of checkpoints represented by an array of integers `nums`, where `nums[i]` represents the speed at index `i`.

The Racer wants to find the maximum total speed obtained during a single "**Perfect Launch**". A "Perfect Launch" is defined as a contiguous subarray of checkpoints where the speed of each checkpoint is `strictly greater` than the previous one.

Your task is to find the **maximum sum** of speeds possible from one such Perfect Launch. The Perfect Launch must include at least one checkpoint.

## Examples

### 1

#### Input
6
10 20 30 5 10 50

#### Output
65

#### Explanation
The The Racer identifies the sequence `[10, 20, 30]` with a sum of 60. However, a better Perfect Launch starts later: `[5, 10, 50]`. This is a strictly increasing contiguous subarray, and its sum is 65.

### 2

#### Input
5
10 20 30 40 50

#### Output
150

#### Explanation
The entire sequence is strictly increasing. The sum is 150.

## Input Format
- The first line contains a single integer `n`, the number of checkpoints.
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
