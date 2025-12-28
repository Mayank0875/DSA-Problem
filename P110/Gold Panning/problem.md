## Title
Gold Panning

## Slug
gold-panning

## Difficulty
Easy

## Description
A prospector pans for gold. A 'Rich Vein' is found when consecutive pans yield strictly more gold dust than the last.

The Prospector is analyzing a sequence of pans represented by an array of integers `nums`, where `nums[i]` represents the gold amount at index `i`.

The Prospector wants to find the maximum total gold amount obtained during a single "**Rich Vein**". A "Rich Vein" is defined as a contiguous subarray of pans where the gold amount of each pan is `strictly greater` than the previous one.

Your task is to find the **maximum sum** of gold amounts possible from one such Rich Vein. The Rich Vein must include at least one pan.

## Examples

### 1

#### Input
6
10 20 30 5 10 50

#### Output
65

#### Explanation
The The Prospector identifies the sequence `[10, 20, 30]` with a sum of 60. However, a better Rich Vein starts later: `[5, 10, 50]`. This is a strictly increasing contiguous subarray, and its sum is 65.

### 2

#### Input
5
10 20 30 40 50

#### Output
150

#### Explanation
The entire sequence is strictly increasing. The sum is 150.

## Input Format
- The first line contains a single integer `n`, the number of pans.
- The second line contains `n` space-separated integers, representing the gold amounts.

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
