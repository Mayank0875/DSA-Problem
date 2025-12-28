## Title
Gym Weight Progression

## Slug
gym-weight-progression

## Difficulty
Easy

## Description
A bodybuilder logs bench press weights. A 'Strength Gain' phase is a series of sessions where the weight lifted strictly increases.

The Bodybuilder is analyzing a sequence of sessions represented by an array of integers `nums`, where `nums[i]` represents the weight (lbs) at index `i`.

The Bodybuilder wants to find the maximum total weight (lbs) obtained during a single "**Strength Gain**". A "Strength Gain" is defined as a contiguous subarray of sessions where the weight (lbs) of each session is `strictly greater` than the previous one.

Your task is to find the **maximum sum** of weight (lbs)s possible from one such Strength Gain. The Strength Gain must include at least one session.

## Examples

### 1

#### Input
6
10 20 30 5 10 50

#### Output
65

#### Explanation
The The Bodybuilder identifies the sequence `[10, 20, 30]` with a sum of 60. However, a better Strength Gain starts later: `[5, 10, 50]`. This is a strictly increasing contiguous subarray, and its sum is 65.

### 2

#### Input
5
10 20 30 40 50

#### Output
150

#### Explanation
The entire sequence is strictly increasing. The sum is 150.

## Input Format
- The first line contains a single integer `n`, the number of sessions.
- The second line contains `n` space-separated integers, representing the weight (lbs)s.

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
