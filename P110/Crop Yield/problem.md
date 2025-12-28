## Title
Crop Yield

## Slug
crop-yield

## Difficulty
Easy

## Description
A farmer harvests rows of corn. A 'Bountiful Patch' is a sequence of rows where the yield strictly increases row by row.

The Farmer is analyzing a sequence of rows represented by an array of integers `nums`, where `nums[i]` represents the bushel count at index `i`.

The Farmer wants to find the maximum total bushel count obtained during a single "**Bountiful Patch**". A "Bountiful Patch" is defined as a contiguous subarray of rows where the bushel count of each row is `strictly greater` than the previous one.

Your task is to find the **maximum sum** of bushel counts possible from one such Bountiful Patch. The Bountiful Patch must include at least one row.

## Examples

### 1

#### Input
6
10 20 30 5 10 50

#### Output
65

#### Explanation
The The Farmer identifies the sequence `[10, 20, 30]` with a sum of 60. However, a better Bountiful Patch starts later: `[5, 10, 50]`. This is a strictly increasing contiguous subarray, and its sum is 65.

### 2

#### Input
5
10 20 30 40 50

#### Output
150

#### Explanation
The entire sequence is strictly increasing. The sum is 150.

## Input Format
- The first line contains a single integer `n`, the number of rows.
- The second line contains `n` space-separated integers, representing the bushel counts.

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
