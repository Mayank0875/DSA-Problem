## Title
Puzzle Solving Time

## Slug
puzzle-solving-time

## Difficulty
Easy

## Description
A speedcuber tracks solve times. A 'Regression' (in this context, viewed as increasing time) is a sequence where solve times strictly increase due to fatigue.

The Cuber is analyzing a sequence of solves represented by an array of integers `nums`, where `nums[i]` represents the time (seconds) at index `i`.

The Cuber wants to find the maximum total time (seconds) obtained during a single "**Fatigue Streak**". A "Fatigue Streak" is defined as a contiguous subarray of solves where the time (seconds) of each solve is `strictly greater` than the previous one.

Your task is to find the **maximum sum** of time (seconds)s possible from one such Fatigue Streak. The Fatigue Streak must include at least one solve.

## Examples

### 1

#### Input
6
10 20 30 5 10 50

#### Output
65

#### Explanation
The The Cuber identifies the sequence `[10, 20, 30]` with a sum of 60. However, a better Fatigue Streak starts later: `[5, 10, 50]`. This is a strictly increasing contiguous subarray, and its sum is 65.

### 2

#### Input
5
10 20 30 40 50

#### Output
150

#### Explanation
The entire sequence is strictly increasing. The sum is 150.

## Input Format
- The first line contains a single integer `n`, the number of solves.
- The second line contains `n` space-separated integers, representing the time (seconds)s.

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
